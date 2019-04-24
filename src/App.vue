<template>
  <div id="app">
    <Navigation/>
    <TextImg class="intro"/>
    <TextImg class="is-curved"/>
    <Concept/>
    <TextImg class="is-curved"/>
  </div>
</template>

<script>
import Navigation from './components/Navigation.vue'
import TextImg from './components/TextImg.vue'
import Concept from './components/Concept.vue'

export default {
  name: 'app',
  components: {
    Navigation,
    TextImg, 
    Concept
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
