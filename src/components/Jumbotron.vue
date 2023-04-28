
<script>
export default {
    name: "Jumbotron"
}
</script>

<template>
  <div class="jumbo"></div>
</template>

<style lang="scss" scoped>

    @use "../scss/partials/utilities" as *;

    .jumbo{
        width: 100vw;
        height: 400px;
        background-image: url("../assets/img/jumbotron.jpg");
        background-size: cover;
        background-repeat: no-repeat;
    }

</style>