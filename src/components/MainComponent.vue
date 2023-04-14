<template>
    <main>
        <div class="container">
            <div class=" row">
                <CardComponent v-for="(card, index) in cards" :key="index" :image="card.thumb" :title="card.series.toLocaleUpperCase()"/>
            </div>  
        </div>
          
  </main>
</template>

<script>
import { cards } from '../data/data.js';
import CardComponent from './CardComponent.vue';
    export default {
        name: 'MainComponent',
        components: {
            CardComponent,
        },
        data() {
            return{
                cards: cards,
            }
        }
    }
</script>

<style lang="scss" scoped>

</style>