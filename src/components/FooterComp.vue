<template>
  <footer>

    <div class="box-sfondo">
      
      <div class="container">

        <div class="col-left">
          <div class="col-primo">
            <h3>Dc Comics</h3>
            <nav>
              <ul>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Comics</a></li>
                <li><a href="#">Movies</a></li>
                <li><a href="#">TV</a></li>
                <li><a href="#">Games</a></li>
                <li><a href="#">Video</a></li>
                <li><a href="#">News</a></li>
              </ul>
            </nav>

            <h3>Shop</h3>
            <nav>
              <ul>
                <li><a href="#">Shop DC </a></li>
                <li><a href="#">Shop DC Collectibles</a></li>
              </ul>
            </nav>
          </div>

          <div class="col-secondo">
            <h3>Dc</h3>
            <nav>
              <ul>
                <li><a href="#">Terms Of Use</a></li>
                <li><a href="#">Privacy policy (New)</a></li>
                <li><a href="#">Ad Choices</a></li>
                <li><a href="#">Advertising</a></li>
                <li><a href="#">Jobs</a></li>
                <li><a href="#">subscription</a></li>
                <li><a href="#">Talent Workshops</a></li>
                <li><a href="#">CPSC Certificates</a></li>
                <li><a href="#">Ratings</a></li>
                <li><a href="#">Shop Help</a></li>
                <li><a href="#">Contact Us</a></li>
              </ul>
            </nav>
          </div>

          <div class="col-terzo">
            <h3>Site</h3>
            <nav>
              <ul>
                <li><a href="#">DC</a></li>
                <li><a href="#">MAD Magazine</a></li>
                <li><a href="#">DC Kids</a></li>
                <li><a href="#">DC Universe</a></li>
                <li><a href="#">DC Power Visa</a></li>
              </ul>
            </nav>
          </div>
        </div>

        <div class="col-right">
          <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>
      </div>
    </div>

    <div class="box-foot">
      <div class="container">

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
  background-image: url(../assets/img/footer-bg.jpg);
  background-size: cover;
  height: 400px;
  overflow: hidden;
}

.box-foot{
  background-color: $fourth-color;
  height: 150px;
  padding-bottom: 20px;
}

.col-left{
  float: left;
  width: 35%;
  padding: 20px 0px;

  .col-primo,
  .col-secondo,
  .col-terzo{
    float: left;
    width: 33%;
    padding: 10px;

    h3{
      color: $primary-color;
      margin: 20px 0px;
    }
    ul{
      list-style: none;

      li{
        a{
          color:$fifth-color;
          @include decor;
          font-size: 0.7rem;
          &:hover{
            text-decoration: underline;
          }
        }
      }
    }
  }

  
}

.col-right{
  width: 55%;
  float: right;
  margin: auto;

  img{
    width: 80%;
    margin-top: -103px;
    margin-left: 100px;
  }
}


</style>