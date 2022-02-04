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
.header{
    height: 12vh;
    margin-top: 1vh;
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
    background-color: ;
}
.searchBox button:hover{
    background-color: ;
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
</style>