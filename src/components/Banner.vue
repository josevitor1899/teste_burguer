<template>
    <div id="main-banner">
        <h1>Make Your Burguer</h1>
    </div>
</template>

<script>
    export default {
       name: "Banner"
    }
</script>

<style scoped>
    #main-banner {
        background-image: url('/public/img/burger.jpg');
        background-position: 0 -250px;
        background-size: cover;
        display: flex;
        align-items: center;
        justify-content: flex-start;
        height: 90vh;
        background-repeat: no-repeat;
    }

    #main-banner h1 {
        color: #fff;
        text-align: center;
        font-size: 60px;
        background-color: #2222;
        padding: 20px 40px;
    }
</style>