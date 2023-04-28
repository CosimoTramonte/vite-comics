<script>
export default {
    name: "Main"
}
</script>

<template>

  <div class="main-container">
    <div class="card-container">
      <div class="tag-series">
        <span>CURRENT SERIES</span>
      </div>
    </div>
  </div>
  
</template>

<style lang="scss" scoped>

  @use "../scss/partials/utilities" as *;
  @use "../scss/partials/mixin" as *;

  .main-container{
    @include centerFlex("vertical");
    background-color: $secondary-color;
    color: white;
    min-height: 150px;

    .card-container{
      width: 80%;
      margin: 0 auto;
      position: relative;

      .tag-series{
        position: absolute;
        background-color: $primary-color;
        padding: 10px;
        bottom: 55px;
      }
    }
  }

</style>