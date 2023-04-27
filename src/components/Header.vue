
<script>
import { MenuNav } from "../data/data.js"

export default {
  name: "Header",

  data(){
    return{
      MenuNav
    }
  }

}
</script>

<template>

  <div class="header-container">
    <img src="../assets/img/dc-logo.png" alt="logo">
    <ul>
      <li v-for="(li,index) in MenuNav" :key="index" :class="{'active' : li.isActive}"><a href="#">{{ li.text }}</a></li>
    </ul>
  </div>

</template>

<style lang="scss" scoped>
  @use "../scss/partials/utilities" as *;
  @use "../scss/partials/mixin" as *;

  .header-container{
    @include centerFlex("vertical");
    justify-content: space-between;
    height: 100px;

    img{
      height: 100%;
      padding: 10px;
    }

    ul{
      @include centerFlex("both");
      height: 100%;

      li {
      list-style: none;
      @include centerFlex("vertical");
      padding: 10px;
      height: 100%;
      border-bottom: 5px solid white;

      &.active {
        border-bottom: 5px solid $primary-color;
        a{
          color: $primary-color;
        }
      }

      a{
        text-decoration: none;
        color: $secondary-color;
        font-size: 13px;
      }
    }
    }
  }

</style>