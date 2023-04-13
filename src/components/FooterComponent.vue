<template>
    <footer>
        <BuyComicsComponent/>
    </footer>
</template>

<script>
import BuyComicsComponent from './BuyComicsComponent.vue';
    export default {
        name: 'FooterComponent',
        components: {
            BuyComicsComponent,
        }
    }
</script>

<style lang="scss" scoped>
footer{
    background-image: url('../assets/images/footer-bg.jpg');
}
</style>