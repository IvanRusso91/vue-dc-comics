<template>
  <main>
    <div class="jumbo">
     <div class="container title"><h2>Current Series</h2></div>
    </div>

    <div class="box-cards">
      <div class="container box-c"> 
        <CardComp
          v-for="(link,index) in linksImg" 
          :key="`link-${index}`"
          :link="link"
        />
      </div>
      
      <div class="btn-box">
        <a class="btn" href="#">Load More</a>
      </div>
      
    </div>
    <div class="box-choice">
      <div class="container">
        <ul>
          <li>
            <a href="#"><img  class="image-a" src="../assets/img/buy-comics-digital-comics.png" alt="loghi-choice"><p>digital comics</p></a>
          </li>

          <li>
            <a href="#"><img  class="image-b" src="../assets/img/buy-comics-merchandise.png" alt="loghi-choice"><p>dc merchandise</p></a>
          </li>

          <li>
            <a href="#"><img  class="image-c" src="../assets/img/buy-comics-subscriptions.png" alt="loghi-choice"><p>subscription</p></a>
          </li>

          <li>
            <a href="#"><img  class="image-d"  src="../assets/img/buy-comics-shop-locator.png" alt="loghi-choice"><p>comic shop locator</p></a>
          </li>

          <li>
            <a href="#"><img  class="image-e" src="../assets/img/buy-dc-power-visa.svg" alt="loghi-choice"><p>dc power visa</p></a>
          </li>
        </ul>
      </div>

    </div>
  </main>
</template>

<script>

import CardComp from '../components/CardComp'
import linksImg from '../assets/data/linksImg'

export default {
  name: 'MainComp',
  components :{
    CardComp
  },
    data(){
      return{
        linksImg,
      }
    },
  mounted(){
    console.log(this.linksImg);
  }
}
</script>

<style  lang="scss" scoped>

@import '../assets/style/vars';
@import '../assets/style/mixin';

 
.jumbo{
  background-image: url(../assets/img/jumbotron.jpg);
  background-size: cover;
  height: 400px;

  .title{
    text-align: left;
    padding-top: 378px;
    text-transform: uppercase;

    h2{
      position: relative;
      @include btn; 
      width: 250px;
    }
  }
}
.box-cards{
  background-color:rgb(28, 28, 28);
  padding: 50px 0px;
  
  .box-c{
    display: flex;
    flex-wrap: wrap;
    
  }
  
  .btn-box{
    display: flex;
    justify-content: center;
    padding-top: 30px ;

    .btn{
      color: $primary-color;
      text-transform: uppercase;
      font-size: 0.8rem;
      display: flex;
      background-color: $third-color;
      padding: 10px 25px;
      color: $primary-color;  
    }
  } 
}


.box-choice{
  background-color: $third-color;
  display: flex;
  align-items: center;

  ul{
    @include menu;
    list-style: none;

    li{
      padding: 50px;
      a{
        @include decor; 
        color: $primary-color;
        font-size: 0.8rem;

        img{
          width: 45px;
        }
        .image-b,
        .image-c{
          width: 55px;
        }
        .image-d{
          width: 35px;
        }
        .image-e{
          margin-top: 15px;
          width: 60px;
        }
        p{
          float: right;
          margin-left: 15px;
          margin-top: 25px; 
        }
      }  
    }
  }
}
</style>