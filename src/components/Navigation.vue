<template>
    <nav class="navigation_container">
        <div class="menuToggle">
            <input class="burger-check" id="burger-check" type="checkbox">
            <label for="burger-check" class="burger"></label>
            
            <picture class="logo">
                <img src="../assets/icons/logo.svg" alt="logo ben">
            </picture>
            
            <ul class="navigation">
                <li><a href="#principle" v-on:click="smoothAnchor">Principe</a></li>
                <li><a href="#core" v-on:click="smoothAnchor">Fonctionnalités</a></li>
                <li><a href="#more" v-on:click="smoothAnchor">Faq</a></li>
            </ul>
        </div>
    </nav>
</template>

<script>
export default {
  name: 'Navigation',
  data: {
      isMobile: false
  },
  props: {
  }, 
  methods: {
      smoothAnchor() {
             document.querySelectorAll('a[href^="#"]').forEach(anchor => {
                anchor.addEventListener('click', function (e) {
                    e.preventDefault();
                    document.querySelector(this.getAttribute('href')).scrollIntoView({
                        behavior: 'smooth'
                    });
                });
            });
      }, 
      stopScroll () {
          document.querySelector('body').classList.add('freeze');
      }
  }
}
</script>

<style lang="scss">
    body.freeze {
        overflow: hidden;
    }
</style>



