<template>
    <div class="principal-container space-y">
        <ul class="side-list dark-grey">
            <li><b>What We Do</b></li>
            <li><b>Degree Programme</b></li>
            <li><b>Career Achievements</b></li>
            <li><b>Personal Menagment</b></li>
            <li><b>Steps To Success</b></li>
            <li><b>Knowledge Transfer</b></li>
        </ul>
        <div class="box-text">
            <h1 class="title-size">Learning Possibilities</h1>
            <p class="txt-base dark-grey">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsa, tempore. Officia maxime incidunt vel beatae sunt quibusdam architecto eius commodi minus, id, repellendus expedita odio et repudiandae, labore magni illum!
                Lorem ipsum dolor sit amet consectetur adipisicing elit.
            </p>
            <ul class="check-list dark-grey">
                <li class="txt-base"><div class="icon">&#10004;</div> <div class="txt">Lorem ipsum dolor </div></li>
                <li class="txt-base"><div class="icon">&#10004;</div> <div class="txt">Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil alias illum obcaecati, ducimus esse excepturi similique.</div></li>
                <li class="txt-base"><div class="icon">&#10004;</div> <div class="txt">Lorem ipsum dolor sit amet consectetur adipisicing elit.</div></li>
                <li class="txt-base"><div class="icon">&#10004;</div> <div class="txt">Lorem ipsum dolor sit amet consectetur adipisicing elit.</div></li>
            </ul>
            <div class="box-img">
                <img src="/images/h12-tabs-icon-1.png" alt="">
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

.principal-container{
    margin-top: 48px;
    display: flex;

    .side-list{
        width: 300px;
        border-bottom: lightgray solid 1px;
        li{
            padding-left: 30px;
            font-size: 18px;
            line-height: 80px;
            border: lightgray solid 1px;
            border-bottom: none;
        }
    }

    .box-text{
        width: 900px;
        padding: 24px;
        position: relative;

        h1{
            margin-bottom: 24px;
        }

        p{
            line-height: 24px;
            margin-bottom: 24px;

        }

        .check-list{
            width: 60%;
            .txt-base{
                padding: 18px 0;
                display: flex;
                align-items: baseline;

                .txt{
                    padding-left: 6px;
                }

                .icon{
                    color: $main-blue;
                }
                
            }
        }

        .box-img{
            position: absolute;
            right: 70px;
            bottom: 0px;
            width: 170px;

            img{
                width: 100%;
            }
        }
    }
}

</style>