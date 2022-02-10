<template>
    <div class="principal-container">
        <div class="box-img">
            <img class="hide" src="/images/h5-client-5-h.png" alt="">
            <img src="/images/h5-client-5.png" alt="">
        </div>
        <div class="box-img">
            <img class="hide" src="/images/h5-client-1-h.png" alt="">
            <img src="/images/h5-client-1.png" alt="">
        </div>
        <div class="box-img">
            <img class="hide" src="/images/h5-client-2-h.png" alt="">
            <img src="/images/h5-client-2.png" alt="">
        </div>
        <div class="box-img">
            <img class="hide" src="/images/h5-client-1-h.png" alt="">
            <img src="/images/h5-client-1.png" alt="">
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
.principal-container{
    padding: 96px 0;
    display: flex;

    .box-img{
        width: 300px;
        position: relative;

        img{
            width: 100%;
        }

        .hide{
            position: absolute;
            top:0;
            left:0;
            display: none;
        }

        &:hover .hide{
            display: block;
        }
    }
}

</style>