<template>
    <div class="header">
        <div class="wrapper">
            <div class="menu">
                <div class="profileImg">
                    <img src="../assets/emblem.png" class="logoImg">
                    <div>
                        <img src="../assets/user.png">
                        <div>Username</div>
                    </div>
                </div>
                <div class="searchBox">
                    <input type="text" placeholder="Search">
                    <button>Search</button>
                </div>
                <div class="navbar">
                    <img src="../assets/home.png" alt="">
                    <img src="../assets/menu.png" alt="">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;1,300;1,400;1,500;1,600;1,700;1,800&display=swap');
.header{
    height: 12vh;
    margin-top: 1vh;
    font-family: 'Open Sans', sans-serif;
}
.wrapper{
    max-width: 1000px;
    margin: 0 auto;
}
.header .wrapper .menu{
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.profileImg
{
    width: 20vw;
    display: flex;
    align-items: center;
    justify-content: space-around;
}
.profileImg:first-child
{
    text-align: center;
    cursor: pointer;
}
.searchBox input{
    width: 18vw;
    border: 1px solid #aaa;
    padding: 8px 8px;
    border-top-left-radius: 4px;
    border-bottom-left-radius: 4px;
}
.searchBox button{
    border: 1px solid #aaa;
    outline: none;
    border-radius: 0px;
    border-top-right-radius: 4px;
    border-bottom-right-radius: 4px;
    padding: 8px 15px;
    background-color: #0EBD60;
    color: white;
    cursor: pointer;
}

.logoImg
{
    width: 4vw;
    margin-right: 20px;
}
.menu .navbar img{
    margin-right: 10px;
    cursor: pointer;
}
@media only screen and (max-width: 768px) {
   .menu{
       justify-content: space-around !important;
       font-size: 0.9em;
   }
}
@media only screen and (max-width: 480px) {
    .menu {
        font-size: 0.8em;
        justify-content: space-evenly !important;
    }
    .menu .profileImg
    {
        display: none;
    }
}
</style>