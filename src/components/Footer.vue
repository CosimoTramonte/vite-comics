<script>
import { MenuFooter } from "../data/data.js"

export default {
    name: "Footer",

    data(){
      return{
        MenuFooter
      }
    }
}
</script>

<template>
  <div class="footerTop-wrapper">
    <div class="footerTop-container">
      <div class="menus">
        <div class="col">
          <h4>DC COMICS</h4>
          <ul>
            <li v-for="(li,index) in MenuFooter.DcComics" :key="index">
              <a :href="li.href">{{ li.text }}</a>
            </li>
          </ul>

          <h4>SHOP</h4>
          <ul>
            <li v-for="(li,index) in MenuFooter.Shop" :key="index">
              <a :href="li.href">{{ li.text }}</a>
            </li>
          </ul>
        </div>
        <div class="col">
          <h4>DC</h4>
          <ul>
            <li v-for="(li,index) in MenuFooter.Dc" :key="index">
              <a :href="li.href">{{ li.text }}</a>
            </li>
          </ul>
        </div>
        <div class="col">
          <h4>SITES</h4>
          <ul>
            <li v-for="(li,index) in MenuFooter.Site" :key="index">
              <a :href="li.href">{{ li.text }}</a>
            </li>
          </ul>
        </div>
      </div>
      <img src="../assets/img/dc-logo-bg.png" alt="dc logo">
    </div>
  </div>

  <div class="footerBottom-wrapper">
    <div class="footerBottom-container">
      <div class="button">
        <span>SIGN-UP NOW!</span>
      </div>
      <div class="social">
        <span>FOLLOW US</span>
        <img src="../assets/img/footer-facebook.png" alt="facebook">
        <img src="../assets/img/footer-twitter.png" alt="twitter">
        <img src="../assets/img/footer-periscope.png" alt="periscope">
        <img src="../assets/img/footer-youtube.png" alt="youtube">
        <img src="../assets/img/footer-pinterest.png" alt="pinterest">
      </div>
    </div>
  </div>


</template>

<style lang="scss" scoped>

  @use "../scss/partials/utilities" as *;
  @use "../scss/partials/mixin" as *;

  .footerTop-wrapper{
    background-image: url("../assets/img/footer-bg.jpg");
    background-repeat: no-repeat;
    background-size: cover;

    .footerTop-container{
      width: 80%;
      margin: 0 auto;
      position: relative;
      display: flex;
      justify-content: space-between;
      min-height: 500px;
      overflow-y: hidden ;
      display: flex;
        align-items: center;

      .menus{
        display: flex;
        align-items: flex-start;
        z-index: 5;

        .col{
          margin-right:35px ;

          h4{
            color: white;
            font-size: 20px;
            margin-bottom: 20px;
          }

          ul{
            list-style: none;
            margin-bottom: 20px;

            li{
              margin: 5px 0;
            
            &:hover a{
              color:white
            }

              a{
                color: #959595;
                text-decoration: none;
              }
            }

          }
        }

      }

      img{
        position: absolute;
        top: -75px;
        zoom: 120%;
        right: 0;
      }
    }
  }
  .footerBottom-wrapper{
    background-color: #303030;
    min-height: 100px;
    @include centerFlex("vertical");
    
    .footerBottom-container{
      width: 80%;
      margin: 0 auto;
      @include centerFlex("vertical");
      justify-content: space-between;

      .button{
        border: 1px solid $primary-color;
        padding: 10px;
        color: white;
      }

      .social{
        @include centerFlex("vertical");

        span{
          color: $primary-color;
          margin-right: 30px;
          font-size: 20px;
          font-weight: bold ;
        }

        img{
          margin: 0 10px;
        }
      }
    }
  }

</style>