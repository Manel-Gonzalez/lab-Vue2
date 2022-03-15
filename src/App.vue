<template>
  <div id="app">
    <Header/>
    <nav>
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </nav>
    <HelloWorld/>
    <router-view/>
    <Footer/>
  </div>
</template>

<script>

import HelloWorld from '@/components/HelloWorld.vue'
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'

export default {
  name:'App',
    components: {
      Header,
      Footer,
      HelloWorld
  },
}

</script>


<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}

.footer-container{
  width: 100%;
  height: 200px;
  background: red;
}
.header-container{
  width: 100%;
 

  background: red;
}

.footer-img{
  width: 100%;
  height: 400px;
}
</style>
