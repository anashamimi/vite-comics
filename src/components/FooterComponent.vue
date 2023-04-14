<template>
    <footer>
        <BuyComicsComponent/>
        <div class="container py-5">
            <div class="d-flex justify-content-between">
                <div class="d-flex gap-5">
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
                    <img src="../../public/images/dc-logo-bg.png" alt="logo bg">
                </div>
                
            </div>
        </div>

        <div></div>
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
    background-image: url('../../public/images/footer-bg.jpg');
    background-size: cover;
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
</style>