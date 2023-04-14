<template>
    <header>
        <div class="container">
            <div class="ah-height py-4 d-flex align-items-center justify-content-between">
                <img src="../../public/images/dc-logo.png" alt="logo dc">
                <ul class="d-flex align-items-center gap-4">
                    <li v-for="(link, index) in links" :key="index">
                        <div>{{ link.text.toUpperCase() }}</div>
                    </li>
                </ul>
            </div>
        </div>
    </header>
    
    
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
        
        background-color: white;
        color: black;

        .ah-height{
            height: 7rem;
        }        

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
                transition: color 0.5s, border-bottom 0.2s;
                &:hover{                   
                    border-bottom: 5px solid rgba(var(--bs-primary-rgb));
                    color: rgba(var(--bs-primary-rgb));
                } 
            }
            
        }
    }
</style>