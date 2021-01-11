<template>
    <div id='image-box'>
        <img src="../assets/pexels-dio-alif-utomo-1897886.jpg" alt="">
    </div> 
</template>

<script>
export default {
    name: 'ImageBox' 
}
</script>

<style scoped>
    #image-box {
        width: 40vw;
        margin: auto;
        height: 70vh;
        background-color: #cb2764;
        box-shadow: -8px -1px 12px 0px rgba(0,0,0,0.51);
        -webkit-box-shadow: -8px -1px 12px 0px rgba(0,0,0,0.51);
        -moz-box-shadow: -8px -1px 12px 0px rgba(0,0,0,0.51);
    }

    img{
        height: 70vh;
        width: 40vw;
        object-fit: cover;
    }

</style>