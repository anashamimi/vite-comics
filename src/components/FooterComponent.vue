<template>
    <footer>
        <BuyComicsComponent/>
        <div class="container ">
            <div class="d-flex justify-content-between">
                <div class="d-flex gap-5 py-5">
                    <div>
                        <ul>
                            <li><h5 class="text-uppercase py-3">dc comics</h5></li>
                            <li><p>Characters</p></li>
                            <li><p>Comics</p></li>
                            <li><p>Movies</p></li>
                            <li><p>TV</p></li>
                            <li><p>Games</p></li>
                            <li><p>Videos</p></li>
                            <li><p>News</p></li>
                        </ul> 

                        <ul>
                            <li><h5 class="text-uppercase py-3">shop</h5></li>
                            <li><p>Shop DC</p></li>
                            <li><p>Shop DC Collectibles</p></li>
                        </ul> 
                    </div>

                    <div>
                        <ul>
                            <li><h5 class="text-uppercase py-3">dc</h5></li>
                            <li><p>Characters</p></li>
                            <li><p>Comics</p></li>
                            <li><p>Movies</p></li>
                            <li><p>TV</p></li>
                            <li><p>Games</p></li>
                            <li><p>Videos</p></li>
                            <li><p>News</p></li>
                            <li><p>TV</p></li>
                            <li><p>Games</p></li>
                            <li><p>Videos</p></li>
                            <li><p>News</p></li>
                        </ul> 
                    </div>

                    <div>
                        <ul>
                            <li><h5 class="text-uppercase py-3">sites</h5></li>
                            <li><p>Characters</p></li>
                            <li><p>Comics</p></li>
                            <li><p>Movies</p></li>
                            <li><p>TV</p></li>
                            <li><p>Games</p></li>
                        </ul>
                        
                    </div>
                    
                </div>

                <div>
                    <img class="ah-logo-bg" src="../../public/images/dc-logo-bg.png" alt="logo bg">
                </div>                
            </div>
        </div>

        <div class="footer-social py-4">
            <div class="container d-flex justify-content-between align-items-center">
                <button type="button" class="btn btn-outline-primary rounded-0 text-uppercase text-white fw-semibold">sign-up now!</button>

                <div class="d-flex gap-3">
                    <p class="text-uppercase fs-5 text-primary fw-bold">follow us</p>
                    <div v-for="(social, index) in socials" :key="index">
                        <img :src="'../../public/images/'+social.image" :alt="social.text">
                    </div>
                </div>
            </div>            
        </div>
    </footer>
</template>

<script>
import { socials } from '../data/data';
import BuyComicsComponent from './BuyComicsComponent.vue';
    export default {
        name: 'FooterComponent',
        components: {
            BuyComicsComponent,
        },
        data() {
            return {
                socials: socials,
            }
        }
    }
</script>

<style lang="scss" scoped>
footer{
    background-image: url('../../public/images/footer-bg.jpg');
    background-size: cover;
    position: relative;
}

ul{
    list-style: none;
    padding: 0;
    margin: 0;
    line-height: 0.5rem;

    p{
        font-size: 0.8rem;
        color: #959595;
    }
}

.ah-logo-bg{
    height: 75%;
    position: absolute;
    margin-left: -40rem;
    margin-top: -2rem;
    z-index: 0;
}

.footer-social{
    background-color: #303030;
    z-index: 100;
    position: relative;

    img{
        cursor: pointer;
    }
}
</style>