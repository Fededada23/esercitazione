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
            
                        <p>{{element.text}}</p>
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>
<style lang="scss">
@use '../styles/partials/variables' as *;
    #main-bottom{
        background-color:$secondaryColor;
            a{
                color:white
    
            }
        }
  
    
</style>