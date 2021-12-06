<template>
    <div class="hero">
        <img src="../assets/movieHero.jpg" alt="">
        <div class="text-container">
            <div class="text">
                <span class="main-heading">Now Streaming</span>
                <h1><span>Now</span>Streaming</h1>
                <a href="#movie-grid" class="button">View Movies</a>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name:'Hero'
    }
</script>

<style scoped>
    .hero{
        height: 400px;
        position: relative;
    }

    .hero::after{
        content: "";
        position: absolute;
        top: 0;
        left: 0;
        height: 100%;
        width: 100%;
        background-color: rgba(0,0,0,0.6);
    }
    img{
        width: 100%;
        height: 100%;
        object-fit: cover;
    }
    h1{
        font-size: 64px;
        font-weight: 200;
        margin-bottom: 8px;
        color: #fff;
    }
    h1 span{
        font-weight: 500;
    }
    .text-container{
        width: 100%;
        height: 100%;
        display: flex;
        justify-content: center;
        flex-direction: column;
        margin: 0;
        top: 0;
        z-index: 99;
        position: absolute;
    }
    .text{
        width: 100%;
        padding: 0 16px;
        max-width: 1400px;
        margin: 0 auto;
    }
    .main-heading{
        font-weight: 600;
        font-size: 18px;
        text-transform: uppercase;
        color: #c92502;
        margin-bottom: 8px;
    }
    .button{
        font-size: 20px;
        align-self: flex-start;
        display: inline-block;
        text-decoration: none;
        color: inherit;
        padding: 8px 16px;
        color: #fff;
        border: none;
        background-color: #c92502;
        border-radius: 4px;
        cursor: pointer;
        transition: 0.3s ease all;
    }
    .button:hover{
        background-color: #891b02;
    }
    @media screen  and (min-width:750px) {
        .hero{
            height: 500px;
        }
        h1{
            font-size: 84px;
        }
    }
</style>