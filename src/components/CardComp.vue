<template>
          
  <div class="card">
    <img :src="link.thumb" :alt="link.type">
    <h3>{{link.series}}</h3>
  </div>
  

</template>

<script>
export default {
  name: 'CardComp',
  props :{
    link: Object,
  },
    mounted(){
    console.log(this.link);
  }
}
</script>

<style lang="scss" scoped>

@import '../assets/style/vars';
@import '../assets/style/mixin';



.card{
  width: 205px;
  margin: 14px;
  margin-bottom: 10px;


  img{
    &:hover{
      cursor: pointer;  
    } 
  }
  h3{
    color: $primary-color;
    margin-top: 10px;
    font-size: 0.9rem;
    width: 200px;
  }
}

</style>