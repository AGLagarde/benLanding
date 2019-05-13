<template>
    <div id="core" class="functions">
        <h2 class="h2">Une mission par semaine<br> pour toi et tes colocs</h2>
       <div class="functions__content">
            <ul>
                <li class="functions__content-item">
                    <div class="functions__content-item--icon">
                        <span><img src="../assets/icons/task.svg" alt=""></span>
                    </div>
                    <div class="functions__content-item--text">
                        <h3 class="h3">Reste organisé</h3>
                        <p>Ben t’aidera à t’organiser grâce à sa liste de tâches et te fera des petits rappels</p>
                    </div>
                </li>
                <li class="functions__content-item">
                    <div class="functions__content-item--icon">
                        <span><img src="../assets/icons/dices.svg" alt=""></span>
                    </div>
                    <div class="functions__content-item--text">
                        <h3 class="h3">Aléatoire mais équitable</h3>
                        <p>Ben répartira les tâches ménagères à tous les membres de la colocation </p>
                    </div>
                </li>
                <li class="functions__content-item">
                    <div class="functions__content-item--icon">
                        <span><img src="../assets/icons/calendar-abs.svg" alt=""></span>
                    </div>
                    <div class="functions__content-item--text">
                        <h3 class="h3">Chaque absence est comptée</h3>
                        <p>Ben prendra en compte les absences de chacun, et t'avertira</p>
                    </div>
                </li>
            </ul>
        </div>
        <div class="functions__illu">
            <picture>
                <img class="homepage" src="../assets/screens/home.svg" alt="">
                <img class="alert" src="../assets/screens/alert-parts.png" alt="">
                <img class="absence" src="../assets/screens/abs-parts.png" alt="">
            </picture>
        </div>
    </div>
</template>

<script>
export default {
  name: 'Concept'
}
</script>


