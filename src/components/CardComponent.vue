<template>
    
        <div class="col-12 col-sm-6 col-md-4 col-lg-3 gy-3">
            <img :src="image" :alt="title" class="img-fluid">
            <p>{{ title }}</p>
        </div>
        
    
</template>

<script>

    export default {
        name: 'CardComponent',
        props: ['image', 'title'],        
    }
</script>

<style lang="scss" scoped>

</style>