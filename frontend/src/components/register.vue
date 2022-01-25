<template>
    <div class="container">
        <form class="registerForm">
            <h1>Register</h1>
            <input type="text"     placeholder="Name">
            <input type="text"     placeholder="Surname">
            <input type="text"     placeholder="Email">
            <input type="password" placeholder="Password">
            <input type="text"     placeholder="Phone Number">
            <input type="submit"   value="Submit">
        </form>
    </div>
</template>

<script>
export default {
    
}
</script>

<style>
.container{
    height: 100vh;
    background-color: #f7ead7;
    display: flex;
    justify-content: center;
    align-items: center
}
.registerForm{
    width: 400px;
    background-color: white;
    border: 1px solid #aaa;
    border-radius: 8px;
    box-shadow: 0px 0px 5px 0px rgb(143 143 143 / 75%);
    display: flex;
    flex-direction: column;
    padding: 20px;
}
.registerForm input{
    margin-bottom: 10px;
    padding: 10px;
    border: 1px solid #aaa;
    border-radius: 8px;
    outline: none;
}
.registerForm input[type=submit] {
    cursor: pointer;
    font-weight: bold;
    border-radius: 25px;
    background-color: #111;
    color: white;
    margin-top: 10px;
}
.registerForm input[type=submit]:hover{
    background-color: rgb(51, 51, 51);
}
@media only screen and (max-width: 768px) {
    .registerForm{
        width: 360px;
        font-size: 0.9em;
    }
}
@media only screen and (max-width: 480px) {
    .registerForm{
        width: 320px;
        font-size: 0.8em;
    }
}
</style>