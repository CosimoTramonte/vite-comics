
<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import SectionMain from "./components/SectionMain.vue";
import Footer from "./components/Footer.vue";


export default {
  name:"App",
  components:{
    Header,
    Main,
    SectionMain,
    Footer
  },
  data(){
    return{
      
    }
  }
}
</script>

<template>
  <Header/>
  <Main/>
  <SectionMain/>
  <Footer/>
</template>

<style lang="scss" scoped>

  @use "./scss/main.scss";


</style>