<template>

               
        <div class="col-12 col-sm-6 col-md-4 col-lg-2 gy-5">
            <div class="ah-card">
                <img :src="image" :alt="title">
                <p>{{ title }}</p>
            </div>
        </div>
        
        
        
    
</template>

<script>

    export default {
        name: 'CardComponent',
        props: ['image', 'title'],        
    }
</script>

<style lang="scss" scoped>
.ah-card{
    height: 15rem;
    width: 12rem;
    margin: 0 auto;

    img{
        height: 100%;
        width: 100%;
    }
}
</style>