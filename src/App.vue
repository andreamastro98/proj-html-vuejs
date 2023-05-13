<script >
  import HeaderComp from './components/HeaderComp.vue';
  import { store } from './store';
  import AdvPerfComp from './components/AdvPerfComp.vue';
  import ResultsComp from './components/ResultsComp.vue';

  export default{
    name:'app',
    components:{
      HeaderComp,
      AdvPerfComp,
      ResultsComp
    },
    data(){
      return{
        store
      }
    },
  }
</script>

<template>
  <HeaderComp/>
  <main>
    <AdvPerfComp style="margin-top: 1000px;"/>
    <ResultsComp/>
  </main>
</template>

<style lang="scss">
@use './style/main.scss';


</style>
