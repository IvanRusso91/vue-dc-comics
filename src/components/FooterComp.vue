<template>
  <footer>

    <div class="box-sfondo">
      
      <div class="container">

        <div class="col-left">
          <div class="col-primo">
            <h3>Dc Comics</h3>
            <nav>
              <ul>
                <li v-for="(comic, index) in comics" :key="`c-${index}`"><a href="">{{comic.name}}</a></li>
              </ul>
            </nav>

            <h3>Shop</h3>
            <nav>
              <ul>
                <li v-for="(object, index) in shop" :key="`d-${index}`"><a href="">{{object.name}}</a></li>
              </ul>
            </nav>
          </div>

          <div class="col-secondo">
            <h3>Dc</h3>
            <nav>
              <ul>
                <li v-for="(oggetto, index) in dc" :key="`e-${index}`"><a href="">{{oggetto.name}}</a></li>
              </ul>
            </nav>
          </div>

          <div class="col-secondo">
            <h3>Site</h3>
            <nav>
              <ul>
                <li v-for="(site, index) in sites" :key="`e-${index}`"><a href="">{{site.name}}</a></li>
              </ul>
            </nav>
          </div>
        </div>

        <div class="col-right">
          <img src="" alt="">
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
  data(){
    return{
      comics:[
        {
          href:'#',
          name: 'Characters',
        },
        {
          href:'#',
          name: 'Comics',
        },
        {
          href:'#',
          name: 'Movies',
        },
        {
          href:'#',
          name: 'TV',
        },
        {
          href:'#',
          name: 'Games',
        },
        {
          href:'#',
          name: 'Videos',
        },
        {
          href:'#',
          name: 'New',
        },
      ],

      shop:[
        {
          href: '#',
          name: 'shop Dc',
        },
        {
          href: '#',
          name: 'shop Dc Collectible',
        },
      ],

      dc:[
        {
          href:'#',
          name: 'Terms of Use',
        },
        {
          href:'#',
          name: 'Privacy policy (New)',
        },
        {
          href:'#',
          name: 'Ad Choices',
        },
        {
          href:'#',
          name: 'Advertising',
        },
        {
          href:'#',
          name: 'Jobs',
        },
        {
          href:'#',
          name: 'Subscriptions',
        },
        {
          href:'#',
          name: 'Talent Workshops',
        },
        {
          href:'#',
          name: 'CPSC Certificates',
        },
        {
          href:'#',
          name: 'Ratings',
        },
        {
          href:'#',
          name: 'Shop Help',
        },
        {
          href:'#',
          name: 'Contact Us',
        },
      ],

      sites:[
        {
          href: '#',
          name: 'DC',
        },
        {
          href: '#',
          name: 'MAD Magazine',
        },
        {
          href: '#',
          name: 'DC Kids',
        },
        {
          href: '#',
          name: 'DC Universe',
        },
        {
          href: '#',
          name: 'DC Power visa',
        },
      ],
    }
  }
}
</script>

<style lang="scss" scoped>

@import '../assets/style/vars';
@import '../assets/style/mixin';

.box-sfondo { 
  background-image: url(../assets/img/footer-bg.jpg);
  background-size: cover;
}

.box-foot{
  background-color: $fourth-color;
  height: 150px;
  padding-bottom: 20px;
}

h3{
  color: $primary-color;
  padding: 10px 0px;
}

.col-left{
  display: flex;
  width: calc(40% / 3);
  padding: 40px 0px;

  .col-primo,
  .col-secondo{
    display: flex;
    flex-direction: column;
    margin-right: 80px;
    
    ul{
      list-style: none;

      li{
        padding: 3px;
      }
      a{
        color:$fifth-color; 
        text-decoration: none; 
        font-size: 0.8rem;
      }
    }
  }
}


</style>