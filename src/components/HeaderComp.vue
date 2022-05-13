<template>
  <header>
    <div class="container box-head">

      <div class="logo">
        <img src="../assets/img/dc-logo.png" alt="">
      </div>

      <div class="right-head">
        <nav>
          <ul>
            <li v-for="(item, index) in menu" :key="`a-${index}`"><a :class="{'active' : item.active}" href="#">{{item.name}}</a></li>
          </ul>
        </nav>
      </div>

    </div>
  </header>
</template>

<script>
export default {
  name:'HeaderComp',
  data(){
    return{
      menu:[
        {
          href: '#',
          name: 'Characters',
          active: false,
        },
        {
          href: '#',
          name: 'Comics',
          active: true,
        },
        {
          href: '#',
          name: 'Movies',
          active: false,
        },
        {
          href: '#',
          name: 'Tv',
          active: false,
        },
        {
          href: '#',
          name: 'Games',
          active: false,
        },
        {
          href: '#',
          name: 'Collectiobles',
          active: false,
        },
        {
          href: '#',
          name: 'Videos',
          active: false,
        },
        {
          href: '#',
          name: 'Fans',
          active: false,
        },
        {
          href: '#',
          name: 'News',
          active: false,
        },
        {
          href: '#',
          name: 'Shop',
          active: false,
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars';
@import '../assets/style/mixin';


.box-head{
  @include  menu;
  padding: 20px 0;
  .logo{
    width: 40%;
    img{
      width: 80px;
    }
  }

  .right-head{
    width: 60%;
    nav{
      margin-right: 10px;

      ul{
        @include menu;
        list-style: none;
        padding-top: 35px;

        li{
          margin-right: 10px;

        }

        a{
          color:$fourth-color; ;
          text-decoration: none;
          text-transform: uppercase;
          font-weight: bold;
          font-size: 0.9rem;
          &.active,
          &:hover{
            color: $third-color;
            border-bottom: 5px solid $third-color;
            padding-bottom: 47px;
          }
            
        }

      }
    }
  }
}

</style>