<template>
   <footer>
     <div class="footer-container">
         <div class="container">

            <!-- row -->
            <div class="row">
                <!-- link -->
                <div class="link">
                    <!-- comics -->
                    <div class="col">
                        <h3>DC Comics</h3>
                        <div class="list">
                            <ul>
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">TV</a></li>
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                            <li><a href="#">News</a></li>
                            </ul>
                        </div>
                        <!-- shop -->
                        <h3>Shop</h3>
                        <div class="list">
                            <ul>
                            <li><a href="#">Shop DC</a></li>
                            <li><a href="#">Shop DC Collectibles</a></li>
                            </ul>
                        </div>
                        <!-- fine shop -->
                    </div>
                    <!-- fine comics -->
                    <!-- dc -->
                    <div class="col">
                        <h3>DC</h3>
                        <div class="list">
                            <ul>
                            <li><a href="#">Terms of Use</a></li>
                            <li><a href="#">Privacy policy (New)</a></li>
                            <li><a href="#">Ad Choices</a></li>
                            <li><a href="#">Advertising</a></li>
                            <li><a href="#">Jobs</a></li>
                            <li><a href="#">Subscriptions</a></li>
                            <li><a href="#">Talent Workshops</a></li>
                            <li><a href="#">CPSC Certificates</a></li>
                            <li><a href="#">Ratings</a></li>
                            <li><a href="">Shop Help</a></li>
                            <li><a href="#">Contact Us</a></li>
                            </ul>
                        </div>
                    </div>
                    <!-- fine dc -->
                    <!-- sites -->
                    <div class="col">
                        <h3>Sites</h3>
                        <div class="list">
                            <ul>
                            <li><a href="#">DC</a></li>
                            <li><a href="#">MAD Magazine</a></li>
                            <li><a href="#">DC Kids</a></li>
                            <li><a href="#">DC Universe</a></li>
                            <li><a href="#">DC Power Visa</a></li>
                            </ul>
                        </div>
                    </div>
                    <!-- fine sites -->
                </div>
                <!-- fine link -->

            <img class="logo-right" src="../assets/img/dc-logo-bg.png" alt="">
        </div>
        <!-- fine row -->
             

         </div>
     </div>

    <!-- icone footer social -->
    <div class="footer-icon">
      <div class="container">
        <div class="row">

          <button>SIGN-UP NOW!</button>

          <div class="social">
            <a href="#">FOLLOW US</a>
            <img src="../assets/img/footer-facebook.png" alt="Facebook">
            <img src="../assets/img/footer-twitter.png" alt="Twitter">
            <img src="../assets/img/footer-youtube.png" alt="YouTube">
            <img src="../assets/img/footer-pinterest.png" alt="Pinterest">
            <img src="../assets/img/footer-periscope.png" alt="Periscope">
          </div>
        </div>
       </div>
    </div>

   </footer>
</template>

<script>
export default {
  name: 'MyFooter'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

    @import "../assets/style/variabili.scss";

    footer {

        // footer container
        .footer-container {
            padding: 30px 0px;
            background-image: url('../assets/img/footer-bg.jpg');
            background-repeat: no-repeat;
            background-size: cover;

            // link
            .link {
                display: flex;

                // col
                .col {
                    width: 170px;

                    h3 {
                        color: $light;
                        text-transform: uppercase;
                        margin: 20px 0px;
                    }

                    // list
                    .list {
                        // ul
                        ul {
                            list-style: none;
                            // li
                            li {
                                margin: 5px 0px;

                                a {
                                    font-size: 12px;
                                    text-decoration: none;
                                    color: #959595;

                                    &:hover {
                                        color: $light;
                                    }
                                }
                            }
                            // fine li
                        }
                        // fine ul
                    }
                    //  fine list
                }
                // fine col
            }
            // fine link

            .logo-right {
                height: 400px;
            }
        }
        // fine footer container

        // footer icon
        .footer-icon {
            background-color: $footerBg;

            // row 
            .row {
                justify-content: space-between;

                button {
                    border: 2px solid $primaryColor;
                    background-color: $footerBg;
                    color: $light;
                    padding: 12px;
                    margin: 20px 0px;
                    font-size: 16px;
                    cursor: pointer;
                }

                .social {
                    display: flex;
                    align-items: center;

                    img {
                        margin: 0px 10px;
                    }

                    a {
                        text-decoration: none;
                        color: $primaryColor;
                        font-weight: bold;
                        margin-right: 5px;
                    }
                }
            }
        }
        // fine footer icon
    }
  
</style>