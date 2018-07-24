<template>
<div>
    <Card v-for="dragon in dragons" v-bind:key="dragon.id" v-bind:dragon="dragon" />
</div>
</template>

<script>
import Card from './Card';

export default {
    name: "CardList",
    components: {
        Card
    },
    data() {
        return {
            dragons: [
            {name: 'Tiamat', 
            id: 1,
            imageUrl: 'https://gbf.wiki/images/thumb/9/94/Tiamat_A.png/480px-Tiamat_A.png'
            }, 
            {name: 'Smaug', 
            id: 2,
            imageUrl: 'https://icdn2.digitaltrends.com/image/the-hobbit-the-desolation-of-smaug-fx-046-640x640.jpg?ver=1.jpg'
            },
            {name: 'Puff', 
            id: 3,
            imageUrl: 'https://assets.pinshape.com/uploads/image/file/111046/container_magic-puff-dragon-3d-printing-111046.jpg'
            }
            ]
        }
    }
}
</script>
<style>
</style>