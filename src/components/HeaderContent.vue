<template>
    <div>
        <img :src="`/images/${content.image}`" alt="">
        <div class="header-text center-x">
            <h1 class="white">{{content.title}}</h1>
            <p class="txt-base white">{{content.text}}</p>
        </div>
    </div>
</template>

<script>
export default {
    props:{
        content:Object
    }
    
}
</script>

<style lang="scss" scoped>
div{
    img{
        width: 100%;
        height: 100%;
        object-fit:cover;
        position: absolute;
        z-index: -1;
        filter:brightness(0.7)
    }

    .header-text{
        width: 70%;
        bottom:300px;
        text-align: center;
        h1{
            font-size: 60px;
        }
        p{
            font-size: 18px;
        }
    }

}

</style>