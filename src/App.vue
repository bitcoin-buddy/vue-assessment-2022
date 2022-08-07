<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/challenge-1">Challenge 1</router-link> | 
      <router-link to="/challenge-2">Challenge 2</router-link> | 
      <router-link to="/challenge-3">Challenge 3</router-link> |
      <router-link to="/final">Final</router-link>
    </div>
    <router-view/>
  </div>
</template>

<script>
    import Home from './views/Home.vue'
    //import Challenge1 from './views/Challenge1.vue'
    //import Challenge2 from './views/Challenge2.vue'
    //import Challenge3 from './views/Challenge3.vue'
    //import Component1 from './components/Component1.vue'
    //import Component2 from './components/Component2.vue'

    export default {
        name: 'app',
        components: {
            Home
        }
    }
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
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
