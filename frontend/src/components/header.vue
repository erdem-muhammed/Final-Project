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
                    <input type="submit" value="Search">
                </div>
                <div class="navbar">
                    <img src="../assets/home.png" alt="">
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
.logoImg
{
    width: 4vw;
}
</style>