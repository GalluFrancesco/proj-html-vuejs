<template>
    <div>
        <img :src="`/images/${content.image}`" alt="">
        <div class="header-text">
            <h1>{{content.title}}</h1>
            <p class="txt-base">{{content.text}}</p>
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
        z-index: 0;
        filter:brightness(0.7)
    }

    .header-text{
        text-align: center;
        z-index: 1;
        position:absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%,-50%);
    }

}

</style>