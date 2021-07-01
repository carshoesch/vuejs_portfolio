<template>
    <!-- Navbar -->
    <Navbar/>
    
    <!-- über mich section mit den skills -->
    <UeberMich/>
        
    <!-- Portfolio Grid-->
    <PortfolioItems/>
        
    <!-- About-->
    <Werdegang/>
    
    <!-- Contact-->
    <ContactMe/>

    <!-- Footer-->
    <Footer/>
    
</template>

<script>

import UeberMich from './components/UeberMich.vue'
import PortfolioItems from './components/PortfolioItems.vue'
import Werdegang from './components/Werdegang.vue'
import Navbar from './components/Navbar.vue'
import ContactMe from './components/ContactMe.vue'
import Footer from './components/Footer.vue'


export default {
  name: 'App',
  components: {
    UeberMich,
    PortfolioItems,
    Werdegang,
    Navbar,
    ContactMe,
    Footer
  }
}
</script>

<style lang="scss" scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* margin-top: 60px; */

  header {
    height: 100vh;
  }

}
</style>
