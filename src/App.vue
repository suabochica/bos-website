<template>
  <div id="app">
    <Header/>
    <Quote/>
    <Principles/>
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Header from './components/Header.vue'
import Quote from './components/Quote.vue'
import Principles from './components/Principles.vue'

export default {
  name: 'app',
  components: {
    HelloWorld,
    Header,
    Quote,
    Principles
  }
}
</script>

<style>
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
