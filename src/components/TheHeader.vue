<template>
  <header>
        <router-link to='/'><img src="../assets/cupcakesandcookies.png" alt="Cupcakes and Cookies logo"></router-link>
        <div class="menu">
            <router-link class="link-icon" to="/"><img src="../assets/house.png" alt="House"></router-link>
            <router-link class="link-icon" to="/"><img src="../assets/compass-arrow.png" alt="Compass"></router-link>
            <router-link class="link-icon" to="/"><img src="../assets/file.png" alt="File"></router-link>
            <router-link class="link-icon" to="/"><img src="../assets/question-mark.png" alt="Question-mark"></router-link>
            <router-link class="link-icon" to="/"><img src="../assets/person.png" alt="Person"></router-link>
        </div>
    </header>
</template>

<script>
export default {
    name: 'TheHeader'
}
</script>

<style>
header {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
}
.link-icon{
    background-color: #ee2961;
    border-radius: 50%;
    padding: 8px;
    min-width: 25px;
    min-height: 25px;
    display: inline-flex;
    justify-content: center;
    margin: 0 3px;
}
</style>