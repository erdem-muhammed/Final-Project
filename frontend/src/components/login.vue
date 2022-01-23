<template>
    <div class="container">
       <div class="loginBox">
           <h1>Sign in</h1>
           <input type="text" placeholder="Username or Email">
           <input type="text" placeholder="Password">
           <input type="submit" value="Login">
            <input type="submit" value="Forgot Password" id="forgotPass">
            <router-link to="/signup" tag="button" id="registerBtn">Register</router-link>
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
.loginBox input {
    border-radius: 8px;
    padding: 10px;
    margin-bottom: 10px;
    border: 1px solid #aaa;
}
.loginBox input[type=submit] {
    cursor: pointer;
    background-color: black;
    color: white;
    font-weight: bold;
    border-radius: 25px;
    width: 100%;
    margin-bottom: 10px;
    margin-top: 5px;
}
#forgotPass
{
    cursor: pointer;
    background-color: white;
    color: black;
    font-weight: bold;
    border-radius: 25px;
    width: 100%;
    margin-bottom: 20px;
}
#registerBtn
{
    cursor: pointer;
    background-color: #0EBD60;
    color: white;
    font-weight: bold;
    border-radius: 25px;
    width: 100%;
    margin-bottom: 20px;
    padding: 10px 15px;
    border: 1px solid #aaa;
}
@media only screen and (max-width: 768px) {
    .loginBox {
        width: 360px;
        font-size: 0.9em;
    }
}
@media only screen and (max-width: 480px) {
    .loginBox {
        width: 300px;
        font-size: 0.8em;
    }
}
</style>