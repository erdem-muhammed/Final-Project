<template>
    <div class="container">
       <div class="loginBox">
           <h3>Sign in</h3>
           <input type="text" placeholder="Username or Email">
           <input type="text" placeholder="Password">
           <input type="submit" value="Login">
       </div>
    </div>
  
</template>

<script>
export default {
    
}
</script>

<style scoped>
.container
{
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #f7ead7;
}
.loginBox {
    padding: 0px 20px 20px 20px;
    display: flex;
    flex-direction: column;
    width: 400px;
    height: 400px;
    background-color: white;
    border-radius: 8px;
    box-shadow: 0px 0px 10px 0px rgb(143 143 143 / 75%);
}
</style>