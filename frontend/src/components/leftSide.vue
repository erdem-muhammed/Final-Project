<template>
    <div class="boxLeft">
        <h2 class="headlineLeft">Groups</h2>
        <div class="row">Chess</div>
        <div class="row">Cooking</div>
        <div class="row">Web Development</div>
    </div>
</template>


<script>
export default {
    
}
</script>

<style>
.boxLeft{
    padding: 15px 10px;
    border: 1px solid #aaa;
    display: flex;
    flex-direction: column;
    text-align: start;
    border-radius: 8px;
    background-color: rgb(129, 231, 235);
    height: 50vh;
}
.headlineLeft{
    cursor: pointer;
}
.row{
    margin-bottom: 40px;
    color: white;
    font-weight: bold;
    cursor: pointer;
    transition: transform ease-in-out 0.3s;
}
.row:hover{
    transform: scale(1.1);
}

</style>