<template>
    <div class="content is-curved">
        <div id="more" class="is-curved__block">
            <div class="content__illu">
                <picture>
                    <img class="homepage" src="../assets/screens/home.svg" alt="homepage">
                    <img class="mission" src="../assets/screens/mission-parts.png" alt="tasks">
                </picture>
            </div>
            <div class="content__body">
                <div class="content__wrap">
                    <h2 class="h2">La démocratie c’est le <br>choix de voter </h2>
                    <p>Ben t’aidera à organiser et donner les tâches ménagére à tout les membres de la colocation de façon parfaitement équitable </p>
                </div>
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
    .is-curved.content {
        z-index: 2;
        height: 975px;
        background-image: url('../assets/background/curve2.svg');
        background-position: left top;
        background-size: cover;
    }
    .content {
        .is-curved__block {
            top: 0;
            height: 100%;
        }
    }
    
    @media screen and (max-width: $tablet) {
        .is-curved {
            &.content {
                height: auto;
                margin-top: 40px;
            }
            .content__illu {
                // flex-basis: 100%;
                // margin: 50px 0 0;
                // height: auto;
                .homepage {
                    // display:block;
                    // width: 85%;
                    // height: auto;
                    // margin: 0 auto;
                }
            }
        }
    }

</style>
