<template>
    <div class="bg-primary text-white py-5">
        <div class="container">
            <ul class="d-flex justify-content-around align-items-center">
                <li v-for="comic in comics" class="d-flex align-items-center gap-2">
                    <img :src="'../../public/images/'+comic.img" :alt="comic.text">
                    <p>{{ comic.text.toUpperCase() }}</p>
                </li>
            </ul>
        </div>
        
    </div>
</template>

<script>
    import {comics} from '../data/data';
    export default {
        name: 'BuyComicsComponent',
        data() {
            return {
                comics: comics,
            }
        }
    }
</script>

<style lang="scss" scoped>

    ul{
        list-style: none;
        margin: 0;

        img{
            height: 50px;
        }

        p{
            margin: 0;
        }
    }

</style>