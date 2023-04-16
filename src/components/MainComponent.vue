<template>
    <main>
        <JumboComponent/>
        
        
        
        <div class="container">

            <div class="ah-current bg-primary text-uppercase fw-bold fs-5 p-2 d-inline-block">
                current series
            </div>

            <div class="row py-4">
                <CardComponent v-for="(card, index) in cards" :key="index" :image="card.thumb" :title="card.series.toLocaleUpperCase()"/>
            </div>  

            <div class="p-5 d-flex justify-content-center">
                <button type="button" class="btn btn-primary rounded-0 px-5 text-uppercase">load more</button>
            </div>
        </div>
          
  </main>
</template>

<script>
import { cards } from '../data/data.js';
import CardComponent from './CardComponent.vue';
import JumboComponent from './JumboComponent.vue';
    export default {
        name: 'MainComponent',
        components: {
            CardComponent,
            JumboComponent,
        },
        data() {
            return{
                cards: cards,
            }
        }
    }
</script>

<style lang="scss" scoped>
.ah-current{
    margin-top: -15px;
}
</style>