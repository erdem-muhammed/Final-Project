<template>
    <div class="">
        <Header />
        <div>
            <div class="wrapper">
                <div class="container">
                    <div class="left">
                        <Groups />
                    </div>
                    <div class="mid">
                        <Flow />
                    </div>
                    <div class="right">

                    </div>

                </div>
            </div>
        </div>
    </div>
        
</template>

<script>
import Header from '../components/header.vue';
import Groups from '../components/leftSide.vue';
import Flow from '../components/userposts.vue';
export default {
    components: {
        Header,
        Groups,
        Flow,
    },
}
</script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;1,300;1,400;1,500;1,600;1,700;1,800&display=swap');
.wrapper{
    max-width: 1000px;
    margin: 0 auto;
}
</style>