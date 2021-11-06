<template>
  <div id="app">
    <Nav-Bar-Item />
    <router-view />
    <div style="margin-top: 50px">
      <Footer-Item />
    </div>
  </div>
</template>

<script>
import FooterItem from './components/Footer-Item.vue'
import NavBarItem from './components/Nav-Bar-Item.vue'
export default {
  components: {
    FooterItem,
    NavBarItem
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Zen+Kurenaido&display=swap');

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
