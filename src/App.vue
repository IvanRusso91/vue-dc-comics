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

@import './assets/style/global';

</style>
