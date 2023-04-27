<script>
export default {
    name: "Main"
}
</script>

<template>

  <div class="main-container">
    <div class="card-container">
      <h1> ---\ Content goes here /--- </h1>
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
    }
  }

</style>