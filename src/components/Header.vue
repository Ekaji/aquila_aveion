<template>
    <div id='header-text'>
        <h1 >{{Name}}</h1>
    </div>
</template>

<script>
export default {
    name: 'HeaderText',
    props: {
        Name: String,
    }
}
</script>

<style scoped>
h1 {
    letter-spacing: 20px;
    font-weight: 100;
}

</style>
