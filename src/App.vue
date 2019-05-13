<template>
  <div id="app">
    <Navigation/>
    <Intro/>
    <Concept/>
    <Functions/>
    <Content class="bis"/>
    <CatchPhrase/>
  </div>
</template>

<script>
import Navigation from './components/Navigation.vue'
import Intro from './components/Intro.vue'
import Functions from './components/Functions.vue'
import Concept from './components/Concept.vue'
import Content from './components/Content.vue'
import CatchPhrase from './components/CatchPhrase.vue'

export default {
  name: 'app',
  components: {
    Navigation,
    Intro, 
    Concept,
    Functions, 
    Content,
    CatchPhrase
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
