<template>
  <div id="app"> 
    <div class="container">
      <div id="logoImg">
        <img src="./assets/logo.jpg" alt="">
      </div>
      <div id="homepage">
        <h1>SHARE</h1>
        <h3>To connect people each other</h3>
              <div id="nav">
                
                <router-link to="/">Home</router-link> |
                <router-link to="/about">About</router-link>
              </div>
      </div>
    </div>
    <router-view/>
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;1,300;1,400;1,500;1,600;1,700;1,800&display=swap');
#app {
  font-family: 'Open Sans', sans-serif;
  height: 100vh;
  background-color: #f7ead7;
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
  border-radius: 8px;
  box-shadow: 0px 0px 5px 0px rgb(143 143 143 / 75%);
  display: flex;
}
#logoImg
{
  width: 50%;
}
#logoImg img
{
  width: 100%;
  border-top-left-radius: 8px;
  border-bottom-left-radius: 8px;
  height: 100%;
}
#homepage
{
  padding: 20px 15px 20px 15px;
  width: 50%;
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
