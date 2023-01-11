<script>
     export default {
        data(){
            return{
                headerLinks:[
                    {
                        label:'Characters',
                        url:'#',
                        active:false
                    },
                    {
                        label:'Comics',
                        url:'#',
                        active:false
                    },
                    {
                        label:'Movies',
                        url:'#',
                        active:false
                    },
                    {
                        label:'Tv',
                        url:'#',
                        active:false
                    },
                    {
                        label:'Games',
                        url:'#',
                        active:false
                    },
                    {
                        label:'Collectibles',
                        url:'#',
                        active:false
                    },
                    {
                        label:'Video',
                        url:'#',
                        active:false
                    },
                    {
                        label:'Fans',
                        url:'#',
                        active:false
                    },
                    {
                        label:'News',
                        url:'#',
                        active:false
                    },
                    {
                        label:'Shop',
                        url:'#',
                        active:false
                    },
                ]
            }
        }
    }
</script>
<template lang="">
    <header>
        <a href="/" class="brand">
            <img src="../assets/images/dc-logo.png">
        </a>
        <nav>
            <ul>
                <li v-for="(link,index) in headerLinks" :key="index">
                    <a :href="link.url" :class="link.active ? 'active' :''">
                        {{link.label}}
                    </a>
                </li>
            </ul>
        </nav>

    </header>    
</template>
<style lang="scss">
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;
    header{
        height: 25vh;
        text-align: center;
        @include center;
        justify-content: space-around;
        img{
            width: 70%;
        }
        
    }

    ul{
        list-style-type: none;
        margin: 2rem 1rem;
        @include center;
        li a{
            display: inline-block;
            padding: 1rem;
            text-decoration: none;
            font-weight: 600;
            transition: background-color 0.3s;
            &.active, &:hover{
                border-bottom: 4px solid $secondaryColor;
            }
            color: $fontColor;
            text-transform: uppercase;
            font-size: .8rem;
            
        }

    }
    
</style>