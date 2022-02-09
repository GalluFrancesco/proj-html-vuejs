<template>

    <div class="bg-img">
        <div class="box-img">
            <img src="/images/testimonials-standard-2.png" alt="">
        </div>
        <p class="txt-base white">
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Excepturi delectus quidem distinctio odit sint magni doloremque necessitatibus eum in nam, ad, ipsa veritatis aut, numquam asperiores? Totam iste dolores qui."
        </p>
        <h2 class="white">Jhon Collins</h2>
        <p class="txt-base white">STUDENT</p>
        <div class="select">
            <div class="dot"></div>
            <div class="dot active"></div>
            <div class="dot"></div>
        </div>
    </div>

</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

.bg-img{
    width: 100%;
    background: url('/images/h5-parallax-img-1.png') no-repeat;
    background-size: cover;
    height: 100vh;
    text-align: center;
    padding: 120px 0;

    .box-img{
        margin: 0 auto;
        height: 120px;
        width: 120px;
        border-radius: 100%;
        margin-bottom: 48px;

        img{
            width: 100%;
        }
    }
    
    p{
        width: 800px;
        margin: 0 auto;
        margin-bottom: 24px;
        line-height: 24px;
    }

    h2{
        margin-bottom: 12px;
    }

    .select{
        padding-top: 24px;
        display: flex;
        justify-content: center;

        .dot{
            height: 15px;
            width: 15px;
            margin: 0 12px;
            border-radius: 100%;
            background-color: white;
            filter: opacity(0.5);
        }

        .active{
            filter: none;
        }
    }
}


</style>