<template>
    <header>
        <img :src="`/images/${content[0].image}`" alt="">
        <div class="header-text">
            <h1>{{content[0].title}}</h1>
            <p>{{content[0].text}}</p>
        </div>
        <div class="select">
            <div></div>
            <div></div>
            <div></div>
        </div>
    </header>
</template>

<script>
export default {
    props:{
        content:Array
    }
    
}
</script>

<style lang="scss" scoped>
header{
    height: 100vh;
    width: 100%;
    position: relative;
    img{
        width: 100%;
        height: 100%;
        object-fit:cover;
        position: absolute;
        z-index: 0;
    }

    .header-text{
        text-align: center;
        z-index: 1;
        position:absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%,-50%);
    }

    .select{
        z-index: 1;
        position:absolute;
        bottom:0;
        left: 50%;
        transform: translate(-50%, 0);
        height: 40px;
        display: flex;
        div{
            margin: 12px;
            width: 20px;
            height: 20px;
            border-radius: 100%;
            border: black solid 1px;
            
            //transform: translate(-50%, 0);
        }
    }
}

</style>