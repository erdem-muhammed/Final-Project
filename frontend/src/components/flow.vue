<template>
    <div class="container">
        <div class="post">
                <Post />
        </div>



    </div>
</template>


<script>
import Post from "./post.vue";
export default {
    components: {
        Post

    }
}
</script>



<style>
.container{
    padding: 20px 30px;
}
</style>