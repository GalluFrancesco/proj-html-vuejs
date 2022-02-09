<template>
    <div>
        <div class="principal-container">
            <h1 class="title-size">The Trusted Name for In-Home Tutoring.</h1>
            <p class="txt-base grey">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sed impedit inventore, quas quae ipsum voluptatibus eveniet sequi quos mollitia cumque quia deserunt! Ipsam quod natus aliquid expedita fuga nemo quasi.</p>
            <p class="txt-base blue">LEARN MORE</p>
            <div class="box-img">
                <img src="/images/h5-img-1.jpg" alt="">
            </div>
        </div>
        <hr>
    </div>
</template>

<script>

export default {

    
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

.principal-container{
    padding-top: 48px;    

    h1{
    width: 50%;
    margin-bottom: 24px;
    }

    p{
    line-height: 24px;
    }

    .grey{
        color: grey;
        margin-bottom: 24px;
    }

    .blue{
        color: $main-blue; 
    }

    .box-img{
        width: 100%;

        img{
            width: 100%;
        }
    }
}


</style>