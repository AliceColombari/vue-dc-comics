<template>

    <main>
        
            <div class="jumbotron">
               <img src="../assets/img/jumbotron.jpg" alt="">
            </div>

            <div class="current-series">
                <div class="container current-series-container">
                    <button class="current-series-btn">CURRENT SERIES</button>
                    <div class="row current-series-row">
                        <SectionCurrentSeries 
                        v-for="currentSerie in currentSeries" 
                        :key="currentSerie.serie"
                        :image="currentSerie.thumb"
                        :title="currentSerie.series"/>

                        <button class="lead-more-btn">LEAD MORE</button>
                    </div>
                </div>
            </div>

            <div class="icons-blue">
                <div class="icon-container">
                    <div class="single-icon-blue">
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                    <span>DIGITAL COMICS</span>
                </div>

                <div class="single-icon-blue">
                    <img src="../assets/img/buy-comics-merchandise.png" alt="">
                    <span>DC MERCHANDISE</span>
                </div>

                <div class="single-icon-blue">
                    <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                    <span>SUBSCRIPTION</span>
                </div>

                <div class="single-icon-blue">
                    <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                    <span>COMIC SHOP LOCATOR</span>
                </div>

                <div class="single-icon-blue">
                    <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                    <span>DC POWER VISA</span>
                </div>

                </div>
            </div>
       
    </main>

</template>

<script>
import SectionCurrentSeries from "./SectionCurrentSeries.vue";

export default {
  name: 'MyMain',
  components: {
      SectionCurrentSeries
  },
  data() {
      return {
          currentSeries: 
          [
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                "price": "$19.99",
                "series": "Action Comics",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                "price": "$3.99",
                "series": "American Vampire 1976",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                "price": "$16.99",
                "series": "Aquaman",
                "type": "graphic novel"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                "price": "$2.99",
                "series": "Batgirl",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                "price": "$3.99",
                "series": "Batman",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                "price": "$2.99",
                "series": "Batman Beyond",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                "price": "$3.99",
                "series": "Batman/Superman",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                "price": "$4.99",
                "series": "Batman/Superman Annual",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                "price": "$5.99",
                "series": "Batman: The Joker War Zone",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                "price": "$6.99",
                "series": "Batman: Three Jokers",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                "price": "$4.99",
                "series": "Batman: White Knight Presents: Harley Quinn",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                "price": "$16.99",
                "series": "Catwoman",
                "type": "graphic novel"
            }
            ]
      }
      
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
// includo con import il file scss delle variabili
@import "../assets/style/variabili.scss";

main {

    .jumbotron img {
      width: 100%;
      height: 400px;
      overflow: hidden;
      object-fit: cover;
      object-position: top;
      display: block;
    }

    .current-series {
        background-color: $mainBg;

        .current-series-container {
        position: relative;

        .current-series-btn {
            position: absolute;
            top: -20px;
            left: 0;
            padding: 10px 20px;
            background-color: $primaryColor;
            color: $light;
            font-weight: bold;
            cursor: pointer;
            font-size: 16px;
            border: 2px solid $primaryColor;

            &:hover {
                background-color: $primaryColorHover;
                border: 2px solid $primaryColorHover;
            }
        }

        .current-series-row {
            width: 100%;
            padding: 30px 0px;
            flex-wrap: wrap;
            justify-content: space-around;

            .lead-more-btn {
                margin-top: 50px;
                padding: 10px 70px;
                background-color: $primaryColor;
                color: $light;
                font-weight: bold;
                cursor: pointer;
                font-size: 16px;
                border: 2px solid $primaryColor;

                &:hover {
                background-color: $primaryColorHover;
                border: 2px solid $primaryColorHover;
            }
            }
        }
        }

    }




    .icons-blue {
        background-color: $primaryColor;
        display: flex;
        justify-content: space-between;
        align-items: center;

    .icon-container {
        display: flex;
        width: 80%;
        max-width: 1200px;
        margin: auto;

        .single-icon-blue{
            display: flex;
            align-items: center;
            margin: $verticalSpace auto;

            &:hover {
               cursor: pointer;
                -webkit-filter: invert(100%);
                color: $dark;
            }

            img {
                height: 40px;
            }

            span {
                color: $light;
                margin-left: 10px;
                font-size: 14px;
            }
        }

    }
        
    }
}
</style>