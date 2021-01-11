<template>
    <div id='socials'>
        <div class="social-cont">
            <ul class="social" v-for='(value, name ) in SocialMedia' :key='value'>
                 <a :href="`https://${name}.com/${value}`"> 
                    <img :src="`https://img.icons8.com/fluent-systems-regular/40/ffffff/${name}.png`"  class="socialicons" :alt="pic"/>
                 </a>
            </ul>
        </div>
    </div> 
</template>

<script>
export default {
    name: 'socials', 
    props: {
        SocialMedia: Array,
    }
}
</script>

<style >
#socials {
    position: absolute;
    right: 40px;
}

.social-cont {
    display: flex;
    justify-content: center;
    flex-direction: column;
    height: 70vh;
}

.social {
    display: flex;
    flex-direction: column;
    list-style-type: none;
}

img.socialicons{
    width: 40px;
    color: #f4d8e2;
}

</style>