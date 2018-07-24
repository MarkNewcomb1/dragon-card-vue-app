<template>
<div class="card">
    <h2>I'm {{dragon.name}}</h2>
    <img :src='dragon.imageUrl'>
</div>
</template>

<script>
export default {
    name: "Card",
    props: ['dragon']
}
</script>
<style scoped>
.card {
    width: 25%;
    border: 1px solid black;
    background: lightgray;
}
.card img {
    max-width: 100%;
}
</style>