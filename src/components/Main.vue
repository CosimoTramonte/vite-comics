<script>
import Card from "../components/partials/Card.vue";
import CardJson from "../data/dc-comics.json"

export default {
    name: "Main",
    components:{
      Card
    },
    data(){
      return{
        CardJson
      }
    }
}
</script>

<template>

  <div class="main-container">
    <div class="card-container">
      <div class="tag-series">
        <span>CURRENT SERIES</span>
      </div>

      <div class="series">

        <Card 
          v-for="(element,index) in CardJson" 
          :key="index"
          :image="element.thumb"
          :title="element.series"
        />

      </div>
    </div>

    <div class="load-more-button">
      <span>LOAD MORE</span>
    </div>
  </div>
  
</template>

<style lang="scss" scoped>

  @use "../scss/partials/utilities" as *;
  @use "../scss/partials/mixin" as *;

  .main-container{
    @include centerFlex("vertical");
    flex-direction: column;
    background-color: $secondary-color;
    color: white;
    min-height: 150px;
    padding-bottom: 40px;

    .card-container{
      width: 80%;
      margin: 0 auto;
      position: relative;
      padding: 50px 0 20px 0;

      .series{
        width: 100%;
        height: 100%;
        @include centerFlex("vertical");
        flex-wrap: wrap;
        justify-content: space-between;

      }
      
      .tag-series{
        position: absolute;
        background-color: $primary-color;
        padding: 10px;
        top: -20px;
      }

    }

    .load-more-button{
      display: inline-block;
      background-color: $primary-color;
      padding: 10px;
    }
  }

</style>