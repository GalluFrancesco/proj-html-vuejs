<template>
    <div class="raw space-y principal-container">
        <div class="subject-card">
            <div class="box-img">
                <img src="/images/h5-custom-icon-1.png" alt="">
            </div>
            <div class="box-title">
                <h3>Laguages</h3>
            </div>
        </div>
        <div class="subject-card">
            <div class="box-img">
                <img src="/images/h5-custom-icon-2.png" alt="">
            </div>
            <div class="box-title">
                <h3>Software</h3>
            </div>
        </div>
        <div class="subject-card">
            <div class="box-img">
                <img src="/images/h5-custom-icon-3.png" alt="">
            </div>
            <div class="box-title">
                <h3>Business</h3>
            </div>
        </div>
        <div class="subject-card">
            <div class="box-img">
                <img src="/images/h5-custom-icon-4.png" alt="">
            </div>
            <div class="box-title">
                <h3>Chemistry</h3>
            </div>
        </div>
        <div class="subject-card">
            <div class="box-img">
                <img src="/images/h5-custom-icon-5.png" alt="">
            </div>
            <div class="box-title">
                <h3>Science</h3>
            </div>
        </div>
        <div class="subject-card">
            <div class="box-img">
                <img src="/images/h5-custom-icon-6.png" alt="">
            </div>
            <div class="box-title">
                <h3>DIY&Craft</h3>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

    .raw{
        display: flex;
        justify-content: space-between;

        .subject-card{
            width: 15%;
            height: 250px;
            padding: 60px 12px;
            background-color: $light-blue;
            border: lightgray solid 1px;
            text-align: center;

            .box-img{
                width: 45%;
                margin: 0 auto;
                margin-bottom: 30px;
                img{
                    width: 100%;
                }
            }
        }
    }
</style>