<template>
    <div class="concept is-curved">
        <div id="principle" class="is-curved__block">
            <div class="concept__content">
                <div class="concept__content-wrap">
                    <span><img src="../assets/icons/calendar.svg" alt="calendar"></span>
                    <h2 class="h2">Ben est équitable <br>et organisé </h2>
                    <p>Ben t’aidera à organiser et donner les tâches ménagères à tous les membres de la colocation de façon parfaitement équitable </p>
                </div>
            </div>
            <div class="concept__illu">
                <picture>
                    <img class="homepage" src="../assets/screens/home.svg" alt="homepage">
                    <img class="mission" src="../assets/screens/mission-parts.png" alt="tasks">
                </picture>
            </div>
        </div>
    </div>
</template>

<script>

export default {
    name: 'Content', 
    components: {
    }
}
</script>



<style lang="scss">
@import '../scss/styles.scss';

.is-curved.concept {
    height: 1095px;
    margin-top: -125px;
    background-image: url('../assets/background/curve1.svg');
    background-position: left top;
    background-size: cover; 
}

@media screen and (max-width: $tablet) {
    .is-curved {
        &.concept {
            height: auto;
            margin: 0;
        }
    }
}


</style>
