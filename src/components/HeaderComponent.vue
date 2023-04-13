<template>
    <div class="container">
        <header class="py-4 d-flex align-items-center justify-content-between">
            <img src="../../public/images/dc-logo.png" alt="logo dc">
            <ul class="d-flex align-items-center gap-4">
                <li v-for="(link, index) in links" :key="index">
                    <div>{{ link.text.toUpperCase() }}</div>
                </li>
            </ul>
        </header>
    </div>
    
</template>

<script>
    import {links} from '../data/data';
    export default {
        name: 'HeaderComponent',
        data() {
            return {
                links: links,
            }
        }
    }
</script>

<style lang="scss" scoped>
    header{
        height: 7rem;
        background-color: white;
        color: black;

        img{
            height: 100%;
        }
    }

    ul{
        list-style: none;
        margin: 0;

        li{
            cursor: pointer;
            margin-bottom: 0;

               

            div{ 
                padding: 41.5px 0;
                &:hover{                   
                    border-bottom: 5px solid rgba(var(--bs-primary-rgb));
                } 
            }
            
        }
    }
</style>