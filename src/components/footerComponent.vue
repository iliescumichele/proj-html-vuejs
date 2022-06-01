<template>
  <footer>
      <div class="container d-flex align-items-center justify-content-center h-100">
        <div class="row row-cols-4 d-flex align-items-center ">
          <div class="col">
            <div class="col-sx ">
              <h3 class="mb-4"><span>NEX</span><span>GEN</span></h3>
              <p>A Functional HTML Template for Corporate &amp; Business</p>
              <div class="incons-and-contacts">
                <div class="phone mt-3">
                  <i class="fa-solid fa-phone"></i>
                  <span>+1 (305) 1234-5678</span>
                </div>
                <div class="mail my-3">
                  <i class="fa-solid fa-envelope"></i>
                  <span>hello@example.com</span>
                </div>
                <div class="address mb-3">
                  <i class="fa-solid fa-location-dot"></i>
                  <span>Main Avenue, 987</span>
                </div>
              </div>
              <a href="#get-in-touch" class="btn my-4">GET IN TOUCH</a>
            </div>
          </div>

          <cardFooter 
            v-for="(cardItem, index) in cardFooterList"
            :key="`cardItem${index}`"
            :cardData="cardItem"
          />

        </div>
      </div>

      <div class="container position-relative">
        <div class="bottom-foot  w-100 d-flex justify-content-between">
          <div class="bottom-foot-sx w-50">
            <p>Enjoy the low price. We are tracking any intention of piracy.</p>
          </div>
          <div class="bottom-foot-dx w-50 clearfix">
            <p class="float-right">&copy; 2020 NEXGEN is Proudly Powered by <a href="#">Codings</a>.</p>
          </div>
        </div>
      </div>
  </footer>
</template>

<script>
import cardFooter from "./components_for_main/cards/cardFooter.vue"

export default {
  name: 'footerComponent',
  components: { cardFooter },
  data(){
    return{
      cardFooterList: [
        {
          "title": "About",
          "links": [
            "The Company",
            "Institutional",
            "Social & Events",
            "Innovations",
            "Environment",
            "Technology"
          ]
        },
        {
          "title": "Transport",
          "links": [
            "Industialized",
            "Chemicals",
            "Package Liquids",
            "Constructions",
            "Laminated Wood",
            "And Others"
          ]
        },
        {
          "title": "Support",
          "links": [
            "Responsability",
            "Terms of use",
            "About Cockies",
            "Privacy Policy",
            "Accesibility",
            "Information"
          ]
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars.scss';

  footer{ 
    height: 700px;
    background-image: url('../assets/img/bg-10.jpg');
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
    position: relative;
  }

  .col-sx{
    color: $colorCube_saltpan;

    span:first-child{ 
      color: $materialDesign_morningGlory;
      background-color: $colorCube_blueLagoonAlpha;
      padding: 6px 5px 6px 20px;
      border-radius: 30px 0 0 30px;
    }

    span:last-chlid{ 
      padding-left: 2px;
    }

    .incons-and-contacts{ 
      color: $colorCube_saltpan;

      i{ 
        margin-right: 12px;
      }
    } 

    .btn{ 
      color: $colorCube_saltpan;
      border: 1px solid $materialDesign_elfGreen;
      padding: 10px 22px;
    }
  }

  .card{
    background-color: $colorCube_saltpanAlpha;
    border-radius: 15px;
    color: white;

    p{
      font-size: 1.4rem;
      font-weight: bold;
    }

    li{
      margin: 10px 0;
      list-style: none;
      a{  
        margin-left: 10px;
        text-decoration: none;
        color: $colorCube_saltpan;
      }
    }
  }

  .bottom-foot{
    position: absolute;
    bottom: 0;
    color: $colorCube_saltpan;

    a{ 
      text-decoration: none;
      color: $materialDesign_elfGreen;
    }

    a:hover{
      text-decoration: underline;
    }

    p{
      margin-bottom: 0;
    }
  }

</style>