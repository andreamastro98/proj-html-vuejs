<script >
  import HeaderComp from './components/HeaderComp.vue';
  import { store } from './store';
  import AdvPerfComp from './components/AdvPerfComp.vue';
  import ResultsComp from './components/ResultsComp.vue';
  import BusinessAreaComp from './components/BusinessAreaComp.vue';
  import ExpertComp from './components/ExpertComp.vue'
  import NewsComp from'./components/NewsComp.vue'
  import NewsLetterComp from './components/NewsLetterComp.vue'
  import MessageComp from './components/MessageComp.vue'
  import FooterComp from './components/FooterComp.vue'

  export default{
    name:'app',
    components:{
      HeaderComp,
      AdvPerfComp,
      ResultsComp,
      BusinessAreaComp,
      ExpertComp,
      NewsComp,
      NewsLetterComp,
      MessageComp,
      FooterComp
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
    <BusinessAreaComp/>
    <ExpertComp/>
    <NewsComp/>
    <NewsLetterComp/>
    <MessageComp/>
  </main>
  <FooterComp/>
</template>

<style lang="scss">
@use './style/main.scss';


</style>
