<script >
  import NavComp from './components/NavComp.vue';
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
  <NavComp/>
</template>

<style lang="scss">
@use './style/main.scss';
</style>
