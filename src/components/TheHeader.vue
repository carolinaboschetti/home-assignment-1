<template>
  <header class="header">
        <router-link to='/'><img class="logo" src="../assets/cupcakesandcookies.png" alt="Cupcakes and Cookies logo"></router-link>
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

<style lang='scss' scoped>
header {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
}
.header {
    display: grid;
    grid-template-rows: repeat(2, 1fr);
    grid-gap: 20px;
    padding: 10px;
}
.logo {
    margin: 0;
}
.menu {
    width: 100%;
        display: grid;
        grid-template-columns: repeat(5, 1fr);
        grid-gap: 10px;
}

@media (min-width: 768px) and (max-width: 1023px) {
  //tablet
    .header {
        grid-template-rows: 1fr;
        grid-template-columns: 1fr 2fr;
        padding: 15px;
    }
}
@media (min-width: 1024px) {
    //desktop
    .header {
        grid-template-areas: 
            'logo . icons';
        grid-template-columns: auto 1fr auto;
        padding: 20px;
    }
    .logo {
        grid-area: logo;
    }
    .menu {
        grid-area: icons;
    }
}

.link-icon {
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