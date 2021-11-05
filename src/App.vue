<template>
  <div id="app">
    <Nav-Bar-Item />
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <router-view/>
    <Footer-Item />
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

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
