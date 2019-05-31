<template>
    <div class="intro">
        <div class="intro__content">
            <h2 class="h2">Ben, le meilleur membre de ta colococation</h2>
            <p>Ben est le colocataire parfait, il résout les conflits de ta colocation, il organise, te rappelle et assigne les tâches pénibles à tout les membres de la colocation.</p>
            <a :href=" `//${url.playstore}` " class="button_gradient">
                <img src="../assets/icons/play.png" alt="play icon">
                <p class="button_gradient-content">
                    <span>Disponible sur </span>
                    <span>Play store</span>
                </p>
            </a>
        </div>
        <div class="intro__illu">
            <picture>
                <img class="homepage" src="../assets/img/ben_01.jpg" alt="illustration">
            </picture>
        </div>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                url: {
                    playstore: 'play.google.com/store'
                }

            }
        }
    }
</script>
