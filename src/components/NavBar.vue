<template>
    <div id='nav-bar'>
        <div id='links'>
            <span class="link"><a href="#">Home</a></span>
            <span class="link"><a href="#">About</a></span>
            <div class="round-image"><img src="../assets/pexels-marko-blazevic-1327405.jpg" alt="image"></div>
            <span class="link"><a href="#">Gallery</a></span>
            <span class="link"><a href="#">Contact</a></span>
        </div>
    </div>
    
</template>

<script>
export default {
    name: 'NavBar'
}
</script>

<style scoped>
    #nav-bar {
        display: flex;
        justify-content: center;
        height: 100px;
        font-size: 20px;
        font-weight: 600;
        letter-spacing: 5PX;
    }
    #links {
        display: flex;
        margin-top: 30px;
        margin-left: 40px;
    }
    .link{
        align-self: center;
    }
    .link > a{
          color: #f4d8e2;
          text-decoration: none;
    }
    #links > span:nth-of-type(2n){
        margin-left: 60px;
    }
    .round-image > img{
        display: flex;
        border-radius: 50px;
        width: 100px;
        height: 100px;
        margin: 0px 60px;
    }


</style>