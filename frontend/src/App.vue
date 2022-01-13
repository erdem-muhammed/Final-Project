<template>
  <div id="app"> 
    <div class="container">
      <div id="logoImg">
        <img src="./assets/logo.jpg" alt="">
      </div>
      <div id="homepage">
        <div class="box">
        <h1>SHARE</h1>
        <h3>To connect people each other for better World</h3>
              <div id="nav">
                <button><router-link to="/login">Login</router-link></button>
                <button><router-link to="/signUp">Register</router-link></button>
              </div>
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
  background-color: #e2d7c5;
  display: flex;
  justify-content: center;
  align-items: center;
}
body {
  margin: 0 !important; 
}
#app .container
{
  height: 100%;
  width: 100%;
  background-color: white;
  display: flex;
}
#logoImg
{
  width: 50%;
  height: 100%;
}
#logoImg img
{
  width: 100%;
  height: 100%;
}
#homepage
{
  width: 50%;
  height: 100%;
}
#homepage .box
{
  padding: 50px;
}
#nav {
  display: flex;
  flex-direction: column;
}
#nav button
{
  border-radius: 25px;
  padding: ;
  outline: none;
  padding: 10px;
  background-color: black;
  margin-bottom: 10px;
  border: 1px solid #aaa;
}
#nav button:first-child:hover
{
  background-color: rgb(51, 51, 51);
  transition: background-color ease-in-out 0.4s;
}
#nav button:last-child
{
  background-color: #0EBD60;
}
#nav button:last-child:hover
{
  background-color: #1eac1e;
  transition: background-color ease-in-out 0.4s;
}

#nav a {
  font-weight: bold;
  color: white;
  text-decoration: none;
}

</style>
