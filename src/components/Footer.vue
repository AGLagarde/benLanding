<template>
  <div class="footer">
    <ul>
      <li class="footer_link"><a href="#">© 2019 Ben Colocation</a></li>
      <li class="footer_link"><a href="#">Termes et conditions</a></li>
      <li class="footer_link"><a :href="`//${url.instagram}`">Instagram</a></li>
    </ul>
  </div>
</template>

<script>
    export default {
        data() {
            return {
                url: {
                    instagram: 'www.instagram.com'
                }

            }
        }
    }
</script>


