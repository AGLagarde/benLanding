<template>
  <div id="app">
    <Navigation/>
    <Intro/>
    <Functions/>
    <Curved />
    <CatchPhrase/>
    <Footer/>
  </div>
</template>

<script>
    import Navigation from './components/Navigation.vue'
    import Intro from './components/Intro.vue'
    import Functions from './components/Functions.vue'
    import Concept from './components/Concept.vue'
    import Curved from './components/Curved.vue'
    import CatchPhrase from './components/CatchPhrase.vue'
    import Footer from './components/Footer.vue'

    export default {
        components: {
            Navigation,
            Intro,
            Concept,
            Functions,
            Curved,
            CatchPhrase,
            Footer
        }
    }
</script>

