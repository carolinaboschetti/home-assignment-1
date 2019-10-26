<template>
  <header>
        <router-link to='/'><img src="../../Assets/cupcakesandcookies.png" alt="Cupcakes and Cookies logo"></router-link>
        <div class="menu">
            <router-link class="link-icon" to="/"><img src="../../Assets/house.png" alt="House"></router-link>
            <router-link class="link-icon" to="/"><img src="../../Assets/compass-arrow.png" alt="Compass"></router-link>
            <router-link class="link-icon" to="/"><img src="../../Assets/file.png" alt="File"></router-link>
            <router-link class="link-icon" to="/"><img src="../../Assets/question-mark.png" alt="Question-mark"></router-link>
            <router-link class="link-icon" to="/"><img src="../../Assets/person.png" alt="Person"></router-link>
        </div>
    </header>
</template>

<script>
export default {
    name: 'TheHeader'
}
</script>

<style>

</style>