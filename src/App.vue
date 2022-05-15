<template>
  <div id="app">

    <HeaderComp />

    <MainComp />
    
    <FooterComp />

  </div>
</template>

<script>

import HeaderComp from "./components/HeaderComp";
import MainComp from './components/MainComp';
import FooterComp from './components/FooterComp';
 
export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp,
    FooterComp,
   
  }
}
</script>

<style lang="scss">

@import './assets/style/general';
@import './assets/style/mixin';
@import './assets/style/utils';
@import './assets/style/vars';


</style>
