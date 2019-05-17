<template>
    <nav class="navigation_container">
        <div class="menuToggle">
            <input class="burger-check" id="burger-check" type="checkbox" v-on:click="stopScroll">
            <label for="burger-check" class="burger"></label>
            <picture class="logo">
                <img src="../assets/icons/logo.svg" alt="logo ben">
            </picture>
            <ul class="navigation">
                <li><a href="#principle" v-on:click="detectDevice">Principe</a></li>
                <li><a href="#core" v-on:click="detectDevice">Fonctionnalités</a></li>
                <li><a href="#more" v-on:click="detectDevice">Faq</a></li>
            </ul>
        </div>
    </nav>
</template>

<script>
export default {
    name: 'Navigation',
    data() {
        return {
            deviceMob: false
        } 
    },
    props: {
    }, 
    methods: {
        // smooth scroll on each anchor 
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
        // prevent scroll when burger menu is active  
        // @todo
        stopScroll () {
            const body = document.querySelector('body')
            if(body.classList.contains('freeze')){
                console.log('contient freeze')
                body.classList.remove('freeze');
                document.querySelector('.burger-check').classList.remove('is-active');
            } else {
                console.log('ajoute freeze')
                body.classList.add('freeze');
                document.querySelector('.burger-check').classList.add('is-active');
            }
        }, 
        detectDevice () {
           // const isMobile = /iPhone|iPad|iPod|Android/i.test(navigator.userAgent)
           if (window.innerWidth <= 800) {
               this.deviceMob = true
               console.log('on stop le scroll')
               this.stopScroll()
           } else {
               console.log('on smooth le  scroll')
               this.smoothAnchor()
           }
        }
    }
}
</script>

<style lang="scss">
    body.freeze {
        overflow: hidden;
    }
</style>



