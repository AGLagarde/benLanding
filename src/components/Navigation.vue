<template>
    <nav class="navigation_container">
        <div class="menuToggle">
            <input class="burger-check" id="burger-check" type="checkbox">
            <label for="burger-check" class="burger"></label>
            
            <picture>
                <img src="../assets/icons/logo.svg" alt="logo ben">
            </picture>
            
            <ul class="navigation">
                <li><a href="#principle">Principe</a></li>
                <li><a href="#core">Fonctionnalités</a></li>
                <li><a href="#more">Faq</a></li>
            </ul>
        </div>
    </nav>
</template>

<script>
export default {
  name: 'Navigation',
  props: {
  }
}
</script>


