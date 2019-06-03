<template>
  <div class="catch">
    <picture class="catch__illu">
      <img src="../assets/img/finale.png" alt="roommates">
    </picture>
    <h2 class="h2">Avec Ben, retrouve l'harmonie <br> de ta colocation</h2>
    <a :href=" `//${url.playstore}`" class="button_gradient">
      <img src="../assets/icons/play.png" alt="play">
      <p class="button_gradient-content">
        <span>Disponible sur </span>
        <span>Play store</span>
      </p>
    </a>
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


