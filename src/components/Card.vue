<script>
    export default{
        name: "Card",
        props: {
            img: String,
            text: String
        }
    }
</script>

<template>   
    <div class="card">
        <div>
           <img :src="img" alt="">
           <h5>{{ text }}</h5>
        </div>
        
    </div>
</template>

<style lang="scss" scoped>
    .card{
        width: calc(100% / 6 - 10px);
        margin-bottom: 30px;
        div{
            width: 183px;
            height: 183px;
            margin-bottom: 5px;
            img{
                width: 100%;
                aspect-ratio: 1;
            }
        } 
    }
        
</style>