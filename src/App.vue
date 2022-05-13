<template>
  <div id="app">

   <HeaderComp />

  </div>
</template>

<script>

import HeaderComp from "./components/HeaderComp";
 
export default {
  name: 'App',
  components: {
    HeaderComp,
   
  }
}
</script>

<style lang="scss">

@import './assets/style/general';
@import './assets/style/mixin';
@import './assets/style/utils';
@import './assets/style/vars';


</style>
