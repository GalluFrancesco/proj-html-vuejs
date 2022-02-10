<template>
    <div>
        <div class="principal-container">

            <div class="title-section">
                <h1 class="title-size">Pricing Plans</h1>
                <p class="txt-base dark-grey">Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam tenetur amet, ratione corrupti nisi tempore quam esse provident sint nulla obcaecati harum placeat hic ipsum architecto beatae! Obcaecati, tenetur. Iusto.</p>
            </div>

            <div class="table dark-grey">
                <ul class="col-1">
                    <li><div class="border-top"></div>
                        <div class="col-title">
                            <div class="box-img"></div>
                            <div class="title">Save up to 40% by paying weekly</div>
                        </div>
                    </li>
                    <li class="txt-base">Number of Courses</li>
                    <li class="txt-base">Time</li>
                    <li class="txt-base">Web Designing</li>
                    <li class="txt-base">Human-Centered Designing</li>
                    <li class="txt-base">Basic Marketing</li>
                    <li class="txt-base">Phyton for Everybody</li>
                    <li class="txt-base">Andrid Developer</li>
                    <li class="txt-base">Business English</li>
                </ul>
                <ul class="col-2">
                    <li><div class="border-top"></div>
                        <div class="col-title">
                            <div class="box-img">
                                <img src="/images/h5-custom-icon-7.png" alt="">
                            </div>
                            <div class="title">Standard</div>
                            <div class="title">$12</div>
                        </div>
                    </li>
                    <li class="txt-base">2</li>
                    <li class="txt-base">15 Days</li>
                    <li v-for="(el,n) in firstCol"
                    :key="n">
                    <span v-if="el" class="main-blue">&#10004;</span>
                    <span v-else>&#10007;</span>
                    </li>
                </ul>
                <ul class="col-3">
                    <li><div class="border-top select"></div>
                        <div class="col-title">
                            <div class="box-img">
                                <img src="/images/h5-custom-icon-8.png" alt="">
                            </div>
                            <div class="title">Professional</div>
                            <div class="title">$59</div>
                        </div>
                    </li>
                    <li class="txt-base">4</li>
                    <li class="txt-base">30 Days</li>
                    <li v-for="(el,n) in secondCol"
                    :key="n">
                        <span v-if="el" class="main-blue">&#10004;</span>
                        <span v-else>&#10007;</span>
                    </li>
                </ul>
                <ul class="col-4">
                    <li><div class="border-top"></div>
                        <div class="col-title">
                            <div class="box-img">
                                <img src="/images/h5-custom-icon-9.png" alt="">
                            </div>
                            <div class="title">Advanced</div>
                            <div class="title">$88</div>
                        </div>
                    </li>
                    <li class="txt-base">6</li>
                    <li class="txt-base">Days</li>
                    <li v-for="(el,n) in thirdCol"
                    :key="n">
                        <span v-if="el" class="main-blue">&#10004;</span>
                        <span v-else>&#10007;</span>
                    </li>
                </ul>
            </div>
            <div class="shop-icons">
                <div class="icon-1">
                    <img src="/images/svg-3.svg" alt="">
                </div>
                <div class="icon-12">
                    <img src="/images/svg-2.svg" alt="">
                </div>
            </div>
            <div class="container txt-base dark-grey">
                <div class="button-container"><div class="button">GET IT NOW</div></div>
                <div class="button-container"><div class="button select-button">GET IT NOW</div></div>
                <div class="button-container"><div class="button">GET IT NOW</div></div>
            </div>
        </div>
        <hr>
    </div>
</template>

<script>
export default {

    data(){
        return{
            firstCol:[1,1,0,0,0,0],
            secondCol:[1,1,1,1,0,0],
            thirdCol:[1,1,1,1,1,1],
        }
    }
    
}
</script>

<style lang="scss" scoped>

@import '../style/variables.scss';

.principal-container{
    padding: 96px 0;
    position: relative;

    .title-section{
        width: 1000px;
        margin: 0 auto;
        text-align: center;
        h1{
            margin-bottom: 24px;
        }

        p{
            margin-bottom: 72px;
        }
    }

    .table{

        display: flex;
        border: lightgrey solid 1px;
        border-right:none;
        border-bottom:none;

        ul{
        width: 300px;
        background-color: white;
            li{
                line-height: 60px;
                border-right: lightgrey solid 1px;
                border-bottom:lightgrey solid 1px;
                text-align: center;
                font-size: 16px;

                &:first-child{
                    height: 200px;
                    line-height: 12px;
                    background-color: #F7FDFF;
                    position: relative;

                    .border-top{
                        position: absolute;
                        height: 5px;
                        width: 100%;
                        top: 0;
                        left: 0;
                        background-color: #D6F2FF;
                    }

                    .select{
                        background-color: $main-blue;
                    }
                }

                .main-blue{
                    color: $main-blue;
                }
            }

            .col-title{
            font-size: 30px;
            line-height: 40px;
            color: black;
            font-weight: bold;
            padding-top: 24px;

                .box-img{
                    height: 80px;
                    margin: 0 auto;

                    img{
                        height: 100%;
                    }
                }
            }
        }
        
        .col-1{
            li{
                text-align: start;
                padding: 0 24px;
                font-weight: bold;

                &:first-child{
                    background-color: white;
                }
            }
        }
    }

    .container{
        display: flex;
        flex-direction: row-reverse;
        align-items: center;
        width: 100%;

        .button-container{
            width: 300px;
            padding: 12px 0;
            border: lightgray solid 1px;
            border-top: none;
            border-right: none;
            background-color: #F7FDFF;

            &:first-child{
                width: 301px;
                border-right: lightgray solid 1px;
            }
            
            .button{
                font-weight: bold;
                width: 120px;
                padding: 8px 0;
                border: lightgray solid 1px;
                margin:0 auto;
                text-align: center;
                font-size: 10px;
                background-color: white;
            }

            .select-button{
                border: transparent solid 1px;
                color: white;
                background-color: $main-blue;
            }
        }
    }

    .shop-icons{
        position: absolute;
        right: -70px;
        top:40%;
        div{
            width: 70px;
            height: 70px;
            padding: 12px;
            background-color: white;
            margin-bottom: 12px;
            img{
                width: 100%;
                height: 100%;
            }
        }
    }

}

</style>