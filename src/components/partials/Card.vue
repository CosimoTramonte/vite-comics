
<script>
export default {
    name:"Card",
    props:{
        image: String,
        title: String
    }
}
</script>

<template>
    <div class="serie">
        <div>
            <img :src="image" :alt="title">
        </div>
        <h5>{{ title }}</h5>
    </div>
</template>

<style lang="scss" scoped>
    .serie{
        width: calc(100% / 6 - 20px);
        aspect-ratio: 2/3;
        display: inline-block;
        margin-bottom: 30px;

        div{
            width: 100%;
            height: 100%;

            img{
                width: 100%;
                height: 100%;
                object-fit: cover;
            }
        }

        h5{
            padding: 10px 0;
            text-align: center;
        }
    }
</style>