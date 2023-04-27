<script>
export default {
    name: "Footer"
}
</script>

<template>
  <div class="footerTop-wrapper">
    <div class="footerTop-container">
      <div class="menus">
        <div class="col">
          <h4>DC COMICS</h4>
          <ul>
            <li><a href="#">Characters</a></li>
            <li><a href="#">Comics</a></li>
            <li><a href="#">Movies</a></li>
            <li><a href="#">TV</a></li>
            <li><a href="#">Games</a></li>
            <li><a href="#">Videos</a></li>
            <li><a href="#">News</a></li>
          </ul>

          <h4>SHOP</h4>
          <ul>
            <li><a href="#">Shop DC</a></li>
            <li><a href="#">Shop DC Collectibles</a></li>
          </ul>
        </div>
        <div class="col">
          <h4>DC</h4>
          <ul>
            <li><a href="#">Characters</a></li>
            <li><a href="#">Comics</a></li>
            <li><a href="#">Movies</a></li>
            <li><a href="#">TV</a></li>
            <li><a href="#">Games</a></li>
            <li><a href="#">Videos</a></li>
            <li><a href="#">News</a></li>
            <li><a href="#">TV</a></li>
            <li><a href="#">Games</a></li>
            <li><a href="#">Videos</a></li>
            <li><a href="#">News</a></li>
          </ul>
        </div>
        <div class="col">
          <h4>DC COMICS</h4>
          <ul>
            <li><a href="#">Characters</a></li>
            <li><a href="#">Comics</a></li>
            <li><a href="#">Movies</a></li>
            <li><a href="#">TV</a></li>
            <li><a href="#">Games</a></li>
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
    display: flex;
    align-items: center;
    
    .footerBottom-container{
      width: 80%;
      margin: 0 auto;
      display: flex;
      align-items: center;
      justify-content: space-between;

      .button{
        border: 1px solid $primary-color;
        padding: 10px;
        color: white;
      }

      .social{
        display: flex;
        align-items: center;

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