<script>
    export default{
        name: "Footer",
        data() {
            return {
                abuotList: [
                    {
                        culo: false,
                        title: 'DC COMICS',
                        items: [
                            {
                                item:'Characters'
                            },
                            {
                                item:'Comics'
                            },
                            {
                                item:'Movies'
                            },
                            {
                                item:'TV'
                            },
                            {
                                item:'Games'
                            },
                            {
                                item:'Videos'
                            },
                            {
                                item:'News'
                            },

                        ]
                    },
                    {
                        culo: true,
                        title: 'SHOP',
                        items: [
                            {
                                item: 'Shop DC'
                            },
                            {
                                item: 'Shop DC Collectibles'
                            }
                        ]
                    },
                    {
                        culo: false,
                        title: 'DC',
                        items: [
                            {
                                item:'Term Of Use'
                            },
                            {
                                item:'Privacy Policy(New)'
                            },
                            {
                                item:'Ad Choices'
                            },
                            {
                                item:'Advertising'
                            },
                            {
                                item:'Jobs'
                            },
                            {
                                item:'Subscriptions'
                            },
                            {
                                item:'Talent Workshops'
                            },
                            {
                                item:'CPSC Certificates'
                            },
                            {
                                item:'Ratings'
                            },
                            {
                                item:'ShopHelp'
                            },
                            {
                                item:'Contact Us'
                            },
                        ]
                    },
                    {
                        culo: false,
                        title:'SITIES',
                        items:[
                            {
                                item:'DC'
                            },
                            {
                                item:'MAP Magazine'
                            },
                            {
                                item:'DC Kids'
                            },
                            {
                                item:'DC Universe'
                            },
                            {
                                item:'DC Power Visa'
                            },

                        ]
                    }
                ]
                
            }   
        }
        
    }
</script>

<template>
    <footer>
        <section id="about">
            <div class="container">
                <div class="box">
                    <div class="col">
                        <div v-for="(elem, index) in abuotList" :key="index" :class="(elem.culo == true) ? 'culo' : 'merda' ">
                            <h2>{{elem.title}}</h2>
                            <ul>
                                <li v-for="(element, i) in elem.items" :key="i">{{ element.item }}</li>
                            </ul>
                        </div> 
                    </div> 
                </div>
                <img src="/img/dc-logo-bg.png" alt="">  
            </div>
        </section>
        <section id="links">
            <div class="container">
                <span id="button">SIGN-UP NOW!</span>
                <div>
                    <strong>FOLLOW US</strong>
                    <img src="/img/footer-facebook.png" alt="">
                    <img src="/img/footer-twitter.png" alt="">
                    <img src="/img/footer-youtube.png" alt="">
                    <img src="/img/footer-pinterest.png" alt="">
                    <img src="/img/footer-periscope.png" alt="">
                </div>
            </div>
        </section>
    </footer>
</template>

<style scoped>
</style>
