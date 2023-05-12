<script >
  import HeaderComp from './components/HeaderComp.vue';
  import { store } from './store';

  export default{
    name:'app',
    components:{
      NavComp,
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
</template>

<style lang="scss">
@use './style/main.scss';
</style>
