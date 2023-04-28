
<script>
export default {
    name: "Jumbotron"
}
</script>

<template>
  <div class="jumbo">
    <img src="../assets/img/jumbotron.jpg" alt="jumbo">
  </div>
</template>

<style lang="scss" scoped>

    @use "../scss/partials/utilities" as *;

    .jumbo{
        width: 100%;
        height: 400px;
        overflow: hidden;

        img{
            width: 100%;
        }
    }

</style>