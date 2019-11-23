<template>
  <div id="app">
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div> -->
    <the-header />
    <router-view />
    <the-footer />
  </div>
</template>
<script>
import TheHeader from './components/TheHeader'
import TheFooter from './components/TheFooter'
export default {
  components: {
    TheHeader,
    TheFooter
  }
}
</script>
<style lang="scss">
body {
    background: red url(assets/background.jpg) 0 0 repeat;
}
#app {
  background-color: #ffffff;
  padding: 0 10px;
  width: 90%;
  margin: 10px auto;
  border-radius: 10px;
  box-shadow: #666666 0px 0px 7px;
  overflow: hidden;
}

@media (min-width: 768px) and (max-width: 1023px) {
  //tablet
  #app {
  width: 80%;
  margin: 15px auto;
  padding: 0 15px;
  }
}
@media (min-width: 1024px) {
  //desktop and TV
  #app {
  padding: 0 20px;
  width: 1000px;
  margin: 20px auto;
  }
}

</style>
