<template>
      <div id="home"> 
    <div class="container">
      <div id="logoImg">
        <img src="../assets/logo.jpg" alt="">
      </div>
      <div id="homepage">
        <div class="box">
        <img src="../assets/emblem.png" id="emblem">
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