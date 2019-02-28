<template>
  <div id="app">
    <Header/>
    <Quote/>
    <Principles/>
    <Services />
    <Contact />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Quote from './components/Quote.vue'
import Principles from './components/Principles.vue'
import Services from './components/Services.vue'
import Contact from './components/Contact.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'app',
  components: {
    Header,
    Quote,
    Principles,
    Services,
    Contact,
    Footer
  }
}
</script>

<style>
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
