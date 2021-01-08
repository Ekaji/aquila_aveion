<template>
    <div id='socials'>
        <ul v-for='value in SocialMedia' :key='value'>
            <li>{{value}}</li>
        </ul>
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

<style scoped>

</style>