<template>
  <nav>
    <router-link :to="{name: 'Home'}">Home</router-link> |
    <router-link :to="{name: 'About'}">About</router-link>|
    <router-link :to="{name: 'Jobs'}">jobs</router-link>
    <!-- <router-link :to="{name: 'JobDetails'}">JobDetails</router-link> -->
  </nav>
  <router-view/>
</template>

<style>
#app {
  font-family: Avenir, Helvetica,  Arial, sans-serif;
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
  text-decoration: none;
  padding: 10px;
  border-radius: .25rem;
}

nav a.router-link-exact-active {
  color: #ffffff;
  background: crimson;
}
</style>
 
