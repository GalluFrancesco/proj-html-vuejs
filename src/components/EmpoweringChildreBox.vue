<template>
    <div class="row principal-container space-y">
        <div class="box-img">
            <img src="/images/h5-img-2.jpg" alt="">
        </div>
        <div class="box-txt">
            <h1 class="title-size">Empowering Children to Reach Their Potential</h1>
            <p class="txt-base">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Commodi ad maxime recusandae praesentium libero, repudiandae quam dicta! Omnis quidem, neque rem, excepturi aspernatur saepe autem quo aliquid hic animi tenetur.</p>
            <div  class="row">
                <div>
                    <h1 class="number-style">168</h1>
                    <h2 class="stories">User Stories</h2>
                </div>
                <div>
                    <h1 class="number-style">347</h1>
                    <h2 class="stories">Events</h2>
                </div>
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

.row{
    display: flex;

    .box-img{
        padding-top: 90px;
        width: 50%;

        img{
            width: 90%;
        }
    }

    .box-txt{
        width: 40%;
        padding-top: 48px;
        
        .title-size{
            margin-bottom: 24px;
        }

        p{
            margin-bottom: 24px;
            line-height: 24px;
        }

        .row{
            display: flex;
            color: $main-blue;

                div{
                    width: 50%;
                    .number-style{
                        font-size: 60px;
                }
            }
        }
    }

}

</style>