<script>
    export default{
        name: "Main",
        data() {
            return {
                menuShop: [
                    {
                        nome: 'DIGITAL COMICS',
                        img: '/img/buy-comics-digital-comics.png'
                    },
                    {
                        nome: 'DC MERCHANDISE',
                        img: '/img/buy-comics-merchandise.png' 
                    },
                    {
                        nome: 'SUBSCRIPTION',
                        img: '/img/buy-comics-subscriptions.png'
                    },
                    {
                        nome: 'COSMIC SHOP LOCATOR',
                        img: '/img/buy-comics-shop-locator.png'
                    },
                    {
                        nome: 'DC POWER VISA',
                        img: '/img/buy-dc-power-visa.svg'
                    }
                ]
                
            }   
        }
        
    }
</script>

<template>
  <main>
    <div id="content">
        <div class="container">
            Content goes Here
        </div>  
    </div>
    <div id="shop">
        <div class="container">
            <div v-for="(elem, index) in menuShop">
                <img src="" alt="">

            </div>
        </div>
    </div>
  </main>
</template>

<style lang="scss" scoped>
</style>
