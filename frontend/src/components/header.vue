<template>
    <div class="header">
        <div class="wrapper">
            <div class="menu">
                <img src="../assets/emblem.png" class="logoImg">
                <div class="searchBox">
                    <input type="text" placeholder="Search">
                    <input type="submit" value="Search">
                </div>
                <div class="profile">
                    <img src="../assets/user.png">
                    <div>Username</div>
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

.logoImg
{
    width: 4vw;
}
</style>