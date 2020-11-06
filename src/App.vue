<template>
  <div id="app" class="container">
      <Menu />
      <Main />  
      <About />
      <Services />
      <Portfolio />
      <Contact />   
  </div>
</template>

<script>
import Menu from './components/Menu.vue'
import Main from './components/Main.vue'
import About from './components/About.vue'
import Services from './components/Services.vue'
import Portfolio from './components/Portfolio.vue'
import Contact from './components/Contact.vue'

export default {
  name: 'App',
  components: {
    Menu,
    Main,
    About,
    Services,
    Portfolio,
    Contact
  }
}
</script>

<style lang="scss">
  @import "assets/scss/_grid.scss";
  @import "assets/scss/_variables.scss";
  @import "assets/scss/_fonts.scss";
  @import "assets/scss/main.scss";
</style>
