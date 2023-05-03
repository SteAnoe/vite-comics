<script>
    export default{
        name: "Header",
        data() {
            return {
                currentActive: 0,
                menuLinks: [
                    {
                        nome: 'CHARACTERS',
                        url: '/',
                        current: false
                    },
                    {
                        nome: 'COMICS',
                        url: '/comics',
                        current: true
                    },
                    {
                        nome: 'MOVIES',
                        url: '/movies',
                        current: false
                    },
                    {
                        nome: 'TV',
                        url: '/tv',
                        current: false
                    },
                    {
                        nome: 'GAMES',
                        url: '/games',
                        current: false
                    },
                    {
                        nome: 'COLLECTIBLES',
                        url: '/collectibles',
                        current: true
                    },
                    {
                        nome: 'VIDEOS',
                        url: '/videos',
                        current: false
                    },
                    {
                        nome: 'FANS',
                        url: '/fans',
                        current: false
                    },
                    {
                        nome: 'NEWS',
                        url: '/news',
                        current: false
                    },
                    {
                        nome: 'SHOP',
                        url: '/shop',
                        current: false
                    }
                ]
            }   
        },
        methods: {
            changeCurrent(index){
                this.currentActive = index
            }
        }
    }
</script>

<template>
  <header>
    <div class="container">
       <div>
            <img src="/img/dc-logo.png" alt="">
        </div>
        <nav>
            <ul>
                <li v-for="(elem, index) in menuLinks" :key="index" @click="changeCurrent(index)" :class="(currentActive == index) ? 'active' : '' ">
                    <a :class="(currentActive == index) ? 'active-bg' : '' "><strong>{{ elem.nome }}</strong></a>
                </li>
            </ul>
        </nav> 
    </div>
  </header>
</template>

<style lang="scss" scoped>

</style>
