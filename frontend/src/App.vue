<template>
  <div id="app"> 
    <div class="container">
       <div id="nav">
          <router-link to="/">Home</router-link> |
         <router-link to="/about">About</router-link>
       </div>
    </div>
    <router-view/>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  height: 100vh;
  background-color: #f7ead7;
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: center;
  align-items: center;
}
body {
  margin: 0 !important; 
}
#app .container
{
  height: 80vh;
  width: 80vw;
  background-color: white;
}

#nav {
  margin: 0;
  padding: 0;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
