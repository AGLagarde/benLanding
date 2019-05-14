<template>
    <div class="anchor">
        <button class="anchor__up" v-on:click="goTop">
           Up
        </button>
    </div>
</template>

<script>
export default {
    data() {
        return {
        }
    }, 
    mounted() {
        window.addEventListener('scroll', this.scrollAppear);
    },
    methods: {
        scrollAppear() {
            if (document.body.scrollTop > 50 || document.documentElement.scrollTop > 50) {
                document.querySelector('.anchor__up').classList.add('appear');
            } else {
                document.querySelector('.anchor__up').classList.remove('appear');
            }
        },
        goTop() {
            const totop = document.documentElement.scrollTop || document.body.scrollTop;
            if (totop > 0) {
                window.requestAnimationFrame(this.goTop);
                window.scrollTo(0, totop - totop / 8);
            }
        }
    }
}
</script>

<style lang="scss">
@import '../scss/styles.scss';
    .anchor {
        &__up {
            position: fixed; 
            bottom: 3%; 
            right: 3%;
            width: 80px;
            height: 45px;
            text-transform: uppercase;
            font-size: 26px;
            color: grey; 
            font-weight: 300; 
            letter-spacing: 2.5px;
            color: black;
            background-color: #FFF;
            border: none;
            outline: none;
            border-radius: 45px;
            box-shadow: 0px 8px 15px rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease 0s;
            cursor: pointer;
            z-index: 3;
            opacity: 0;

            &:hover {
                background-color: $redish;
                box-shadow: 0px 15px 20px rgba(249, 31, 76, 0.4);
                color: #FFF;
                transform: translateY(-7px);
            }
        }
        .appear {
            opacity: 1;
        }
    }
</style>
