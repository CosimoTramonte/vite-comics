<script>
export default {
    name: "SectionMain"
}
</script>

<template>

  <div class="sectionmain-container">
    <div class="items-container">
      <ul>
        <li>
          <img src="../assets/img/buy-comics-digital-comics.png" alt="digital comics">
          <a href="#">DIGITAL COMICS</a>
        </li>
        <li>
          <img src="../assets/img/buy-comics-merchandise.png" alt="merch">
          <a href="#">DC MERCHANDISE</a>
        </li>
        <li>
          <img src="../assets/img/buy-comics-subscriptions.png" alt="sub">
          <a href="#">SUNSCRIPTION</a>
        </li>
        <li>
          <img src="../assets/img/buy-comics-shop-locator.png" alt="shop locator">
          <a href="#">COMIC SHOP LOCATOR</a>
        </li>
        <li>
          <img src="../assets/img/buy-dc-power-visa.svg" alt="power visa">
          <a href="#">DC POWER VISA</a>
        </li>
      </ul>
    </div>
  </div>

</template>

<style lang="scss" scoped>

  @use "../scss/partials/utilities" as *;

  .sectionmain-container{
    display: flex;
    align-items: center;
    background-color: $primary-color;
    color: white;
    min-height: 150px;

    .items-container{
      width: 80%;
      margin: 0 auto;

      ul{
        display: flex;
        align-items: center;
        justify-content: space-around;
        flex-wrap: wrap;
        list-style: none;

        li{
          display: flex;
          align-items: center;

          img{
            height: 50px;
            margin-right: 8px;
          }

          &:last-child{
            img {
              width: 60px;
            } 
          }
          
          a{
            text-decoration: none;
            color: white;
          }
        }
      }
    }
  }

</style>