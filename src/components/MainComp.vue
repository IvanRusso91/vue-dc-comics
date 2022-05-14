<template>
  <main>
    <div class="box-cards">
      
      <div class="container ">
        <h1><i class="fa-solid fa-arrow-right"> </i>Content goes here<i class="fa-solid fa-arrow-left"></i></h1>
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
export default {
  name: 'MainComp',
}
</script>

<style  lang="scss" scoped>
@import '../assets/style/vars';
@import '../assets/style/mixin';
.box-cards{
  background-color:$secondary-color ;
  height: 160px;
  
  h1{
    color: $primary-color;
    padding-top: 65px;
  }
  i{
    padding: 0px 15px;
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