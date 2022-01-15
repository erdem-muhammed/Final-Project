<template>
  <div id="app"> 
    <div class="container">
      <div id="logoImg">
        <img src="./assets/logo.jpg" alt="">
      </div>
      <div id="homepage">
        <div class="box">
        <img src="./assets/emblem.png" id="emblem">
        <h1>SHARE</h1>
        <h3>To connect people each other for the better World</h3>
              <div id="nav">
                <router-link to="/login" tag="button">Login</router-link>
                <router-link to="/signup" tag="button">Register</router-link>
              </div>
        </div>
      </div>
      <div class="copyright">
            Copyright © 2022 SHARE, GmbH.
      </div>
    </div>
    <router-view/>
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;1,300;1,400;1,500;1,600;1,700;1,800&display=swap');
#app {
  font-family: 'Open Sans', sans-serif;
  height: 110vh;
}
body {
  margin: 0 !important; 
}
#app .container
{
  height: 100vh;
  width: 100%;
  background-color: white;
  display: flex;
  flex-wrap: wrap;
}
#logoImg
{
  width: 50%;
  height: 100vh;
}
#logoImg img
{
  width: 100%;
  height: 100%;
}
#homepage
{
  width: 50%;
  height: 100vh;
}
#homepage .box
{
  padding: 50px;
}
#emblem
{
  width: 6em;
  height: 6em;
}
#nav {
  display: flex;
  flex-direction: column;
}
#nav button
{
  border-radius: 25px;
  outline: none;
  padding: 10px;
  background-color: black;
  margin-bottom: 10px;
  border: 1px solid #aaa;
  cursor: pointer;
  width: 70%;
  color: white;
  font-weight: bold;
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
.container .copyright
{
  width: 100%;
  height: 10vh;
  display: flex;
  align-items: center;
  justify-content: center;
}

@media only screen and (max-width: 768px) {
  #app
  {
    font-size: 0.9em;
  }
}
@media only screen and (max-width: 480px) {
  #app
  {
    font-size: 0.8em;
    height: 100vh;
  }
  #logoImg 
  {
    display: none;
  }
  #homepage {
    width: 100%;
    
  }
  #homepage .box
  {
    text-align: center;
  }
  #nav{
    align-items: center;
  }
}

</style>
