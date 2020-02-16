<template>
<div class="app">
    <NavBar/>
    <HomePage/>
   <router-view />
    </div>

</template>

<script>
import NavBar from './components/NavBar.vue'
import HomePage from './components/HomePage.vue'
export default {
  name: 'App',
  components:{
    NavBar,HomePage
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
