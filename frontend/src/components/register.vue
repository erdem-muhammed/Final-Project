<template>
    <div class="container">
        <form class="registerForm">
            <h1>Register</h1>
            <input type="text"     placeholder="Name" v-model="reg_name" required>
            <input type="text"     placeholder="Surname" v-model="reg_surname" required>
            <input type="text"     placeholder="Email" v-model="reg_email" required>
            <input type="password" placeholder="Password" v-model="reg_pass" required>
            <input type="text"     placeholder="Phone Number" v-model="reg_phone" required>
            <input type="submit"   value="Submit" @click="register">
        </form>
    </div>
</template>

<script>
export default {
    data(){
        return{
            reg_name: "",
            reg_surname: "",
            reg_email: "",
            reg_pass: "",
            reg_phone: "",
        };
    },
    methods: {
        register(){
            const formData = new FormData();
            formData.append("name", this.reg_name);
            formData.append("surname", this.reg_surname);
            formData.append("email", this.reg_email);
            formData.append("password", this.reg_pass);
            formData.append("phone", this.reg_phone);
            fetch('http://localhost/final_project/register.php',{
                method: 'post',
                mode: 'cors',
                body: formData,
                headers: {
                    'Accept': 'application/json',
                    'Content-Type': 'application/json'
                }
            })
        }
    }
    
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