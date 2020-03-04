<template>
  <div id="app">
    <Navigation />
    <HelloWorld />
    <Category />   
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import Navigation from './components/Navigation'
import Category from './components/Category'



export default {
  name: 'App',
  components: {
    Navigation,
    HelloWorld,
    Category
  }
}
</script>

<style>
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale; 
}
</style>
