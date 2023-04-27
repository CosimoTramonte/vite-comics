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

  .main-container{
    display: flex;
    align-items: center;
    background-color: $secondary-color;
    color: white;
    min-height: 150px;

    .card-container{
      width: 80%;
      margin: 0 auto;
    }
  }

</style>