<template>
    <div>
        <div class="principal-container">
            <div class="title-section">
                <h1 class="title-size">Popular Online Courses</h1>
                <p class="txt-base dark-grey">Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam tenetur amet, ratione corrupti nisi tempore quam esse provident sint nulla obcaecati harum placeat hic ipsum architecto beatae! Obcaecati, tenetur. Iusto.</p>
            </div>
            <div class="cards-container">
                <div class="card-course">
                    <div class="box-img">
                        <img src="/images/course-5-f-img.jpg" alt="">
                    </div>
                    <div class="box-txt">
                        <div class="box-title">
                            <div class="title"><b>Android Developer</b></div>
                            <div class="box-price free txt-base white">FREE</div>
                        </div>
                        <p class="name txt-base">David Sanders</p>
                        <p class="content txt-base dark-grey">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quo voluptatibus quas modi mollitia officiis, corporis dolore ex ut consequuntur? Non dolore exercitationem esse similique corporis iure harum possimus ab id.</p>
                        <div class="txt-base icons-box ">
                            <span><i class="fas fa-user"></i> 1</span> 
                            <span><i class="fas fa-tag"></i> PROGRAMMING</span>
                        </div>
                    </div>
                </div>

                <div class="card-course">
                    <div class="box-img">
                        <img src="/images/course-6-f-img.jpg" alt="">
                    </div>
                    <div class="box-txt">
                        <div class="box-title">
                            <div class="title"><b>Web Designing</b></div>
                            <div class="box-price free txt-base white">FREE</div>
                        </div>
                        <p class="name txt-base">Jennifer Powell</p>
                        <p class="content txt-base dark-grey">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quo voluptatibus quas modi mollitia officiis, corporis dolore ex ut consequuntur? Non dolore exercitationem esse similique corporis iure harum possimus ab id.</p>
                        <div class="txt-base icons-box ">
                            <span><i class="fas fa-user"></i> 1</span> 
                            <span><i class="fas fa-tag"></i> PROGRAMMING</span>
                        </div>
                    </div>
                </div>

                <div class="card-course">
                    <div class="box-img">
                        <img src="/images/course-12-f-img.jpg" alt="">
                    </div>
                    <div class="box-txt">
                        <div class="box-title">
                            <div class="title"><b>Financial Modelling</b></div>
                            <div class="box-price  txt-base white">$20</div>
                        </div>
                        <p class="name txt-base">Edward Bowman</p>
                        <p class="content txt-base dark-grey">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quo voluptatibus quas modi mollitia officiis, corporis dolore ex ut consequuntur? Non dolore exercitationem esse similique corporis iure harum possimus ab id.</p>
                        <div class="txt-base icons-box ">
                            <span><i class="fas fa-user"></i> 1</span> 
                            <span><i class="fas fa-tag"></i> PROGRAMMING</span>
                        </div>
                    </div>
                </div>
            </div>
            <div class="select">
                <div class="dot"></div>
                <div class="dot active"></div>
                <div class="dot"></div>
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
    padding: 96px 0;
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

    .cards-container{
        display: flex;
        justify-content: space-between;
        .card-course{
            width: 30%;
            background-color: white;
            border: lightgray solid 1px;
            .box-img{
                width: 100%;

                img{
                    width: 100%;
                }
            }

            .box-txt{
                padding: 24px;

                .box-title{
                    display: flex;
                    align-items: center;
                    margin-bottom: 6px;

                    .title{
                        flex-grow: 1;
                        font-size: 20px;
                    }

                    .box-price{
                        width: 50px;
                        height: 20px;
                        border-radius: 10px;
                        background-color: $main-blue;
                        font-size: 12px;
                        text-align: center;
                        line-height: 20px;
                    }

                    .free{
                        background-color: #ffd740;
                    }
                }
                
                .name{
                    margin-bottom: 12px;
                    color:#ababab;
                }

                .content{
                    margin-bottom: 12px;
                }

                .txt-base{
                    font-size: 14px;
                }
            }

            .icons-box{
                color:#ababab;

                span{
                    font-size: 11px;
                    margin-right: 6px;
                    .fa-tag{
                        margin-left: 10px;
                    }
                }
               
            }

        }

        
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
            background-color: $main-blue;
            filter: opacity(0.5);
        }

        .active{
            filter: none;
        }
    }

}

</style>