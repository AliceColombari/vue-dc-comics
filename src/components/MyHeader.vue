<template>
  <header>
      <div class="container">
          <div class="header-wrapper">
            <!-- logo -->
            <div class="logo">
              <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <!-- fine logo -->
            <!-- menu -->
            <nav>
              <ul class="menu">
                <li v-for="(link, index) in links" :key="index">
                  <a :href="link.url" :class="{'active' : link.current }">{{link.text}}</a>
                </li>
                <!-- <li><a class="active" href="#">Comics</a></li>
                <li><a href="#">Movies</a></li>
                <li><a href="#">Tv</a></li> 
                <li><a href="#">Games</a></li>
                <li><a href="#">Collectibles</a></li>
                <li><a href="#">Videos</a></li>
                <li><a href="#">Fans</a></li>
                <li><a href="#">News</a></li>
                <li><a href="#">Shop</a></li> -->
              </ul>
            </nav>
            <!-- fine menu -->
          </div>
      </div>
  </header>
</template>

<script>
export default {
  name: "MyHeader",
  data() {
    return {
      links: [
        {
          text: 'Characters',
          url: '#',
          current: false,
        },
        {
          text: 'Comics',
          url: '#',
          current: true,
        },
        {
          text: 'Movies',
          url: '#',
          current: false,
        },
        {
          text: 'TV',
          url: '#',
          current: false,
        },
        {
          text: 'Games',
          url: '#',
          current: false,
        },
        {
          text: 'Collectibles',
          url: '#',
          current: false,
        },
        {
          text: 'Videos',
          url: '#',
          current: false,
        },
        {
          text: 'Fans',
          url: '#',
          current: false,
        },
        {
          text: 'News',
          url: '#',
          current: false,
        },
        {
          text: 'Shop',
          url: '#',
          current: false,
        },
      ]
    }
  }
  
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  // includo con import il file scss delle variabili
  @import "../assets/style/variabili.scss";

  header {

    .header-wrapper {
      display: flex;
      justify-content: space-between;
      align-items: center;
      height: 100px;
    }

    .logo {
      img {
        width: 80%;
      }
    }

    .menu {
      display: flex;

      li {
        margin-left: 20px;
        list-style: none;

        a {
          display: inline-block;
          font-size: 16px;
          text-decoration: none;
          text-transform: uppercase;
          font-weight: bold;
          // metti stessi px della linea per non fare alzare il testo
          line-height: 96px;
          color: $dark;

          &.active,
          &:hover {
            color: $primaryColor;
            border-bottom: 4px solid $primaryColor;
            line-height: 96px;
          }
        }
      }
    }
  }
 
</style>