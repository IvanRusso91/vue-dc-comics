<template>
  <footer>

    <div class="box-sfondo">
      <img src="../assets/img/footer-bg.jpg" alt="">
      <div class="container">

      </div>

      <div class="box-foot">
        <div class="container">

        </div>
      </div>
    </div>

    
    
  </footer>
</template>

<script>
export default {
  name:'FooterComp',
}
</script>

<style lang="scss" scoped>

@import '../assets/style/vars';
@import '../assets/style/mixin';

.box-sfondo {
  
  img{
    position: relative;
    width: 100%;
    background-size: cover;
    background-position: center ;
  }

}

.box-foot{
  background-color: $fourth-color;
  height: 150px;
  padding-bottom: 20px;
}



</style>