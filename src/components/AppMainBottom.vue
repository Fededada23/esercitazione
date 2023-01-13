<script>
    export default {
        data(){
            return{
                mainBottomLinks: [
                    {
                        text: 'Digital Comics',
                        url: '#',
                        image: 'buy-comics-digital-comics.png'
                    },
                    {
                        text: 'Merchandise',
                        url: '#',
                        image: 'buy-comics-merchandise.png'
                    },
                    {
                        text: 'Shop Locator',
                        url: '#',
                        image: 'buy-comics-shop-locator.png'
                    },
                    {
                        text: 'Subscriptions',
                        url: '#',
                        image: 'buy-comics-subscriptions.png'
                    },
                    {
                        text: 'Power Visa',
                        url: '#',
                        image: 'buy-dc-power-visa.svg'
                    }
                ]
            }
        }     
    }
</script>
<template lang="">
    <div id="main-bottom">
        <div class="container">
            <ul>
                <li v-for="(element, index) in mainBottomLinks" :key="index">
                    <a :href="element.url">
                        <img :src="`/images/${element.image}`">
                        <p>{{element.text}}</p>
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>
<style lang="scss">
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;
    #main-bottom{
        background-color:$secondaryColor;
        ul{
            list-style-type: none;
            
            @include center;
            li a{
                text-align: center;
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
                    img{
                        width: 60px;
                        height: 70px;
                    }
            }
            
            
        }
            a{
                color:white
    
            }
        }
  
    
</style>