<template>
  <div id="nav">

    <Header />
    
   
  </div>
  <router-view/>
  <Footer />
</template>

<script>
import Header from "./components/Header.vue"
import Footer from "./components/Footer.vue"

export default {
  components:{
    Header,
    Footer,
  },
}
</script>

