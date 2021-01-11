<template>
    <div id='header'>
        <h1 >{{Name}}</h1>
    </div>
</template>

<script>
export default {
    name: 'Name',
    props: {
        Name: Array,
    }
}
</script>

<style scoped>
h1 {
    letter-spacing: 20px;
    font-weight: 100;
}

</style>
