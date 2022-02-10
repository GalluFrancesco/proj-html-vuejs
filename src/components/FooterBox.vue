<template>
    <footer>
        <div class="principal-container">
            <div class="lists-container">
                <ul class="col-1">
                    <li>
                        <img src="/images/logo-light.png" alt="">
                    </li>
                    <li>
                        <div class="dark-grey">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Modi porro iure nemo, voluptate, fugiat blanditiis neque reiciendis autem asperiores tempore laudantium officia.</div>
                    </li>
                    <li>
                        <div class="light-grey"><i class="fas fa-phone dark-grey"></i> 1-677-234-456</div>
                    </li>
                    <li>
                        <div class="light-grey">
                            <i class="fas fa-clock  dark-grey"></i>  Mon-Sat 8.00-18.00
                        </div>
                    </li>
                </ul>
        
                <ul class="col-2">
                    <li><h4>Popular Courses</h4></li>
                    <li class="dark-grey">
                        <div class="course">Business English</div>
                        Tizio
                    </li>
                    <li class="dark-grey">
                        <div class="course">Social Computing</div>
                        Caio
                    </li>
                    <li class="dark-grey">
                        <div class="course">Learn Spanish</div>
                        Sempronio
                    </li>
                </ul>

                <ul class="col-3">
                    <li><h4>Support</h4></li>
                    <li v-for="(el,n) in supportList"
                    :key="n"
                    class="dark-grey">{{el}}</li>
                </ul>

                <ul class="col-4">
                    <li><h4>Flexible Learning</h4></li>
                    <li class="img">
                        <img src="/images/footer-img-1.png" alt="">
                    </li>
                </ul>
            </div>
            <hr>
            <div class="copy dark-grey">
                Copyright2017 MikadoTheme
            </div>
        </div>

    </footer>
</template>

<script>
export default {
    props:{
        supportList: Array
    }
    
}
</script>

<style lang="scss" scoped>

footer{
    background-color: black;
    .principal-container{
        .lists-container{
            padding-top:46px;
            width: 100%;
            display: flex;

            .col-1{
                img{
                    height: 30px;
                }
            }
            
            ul{ 
                width: 20%;
                color:white;
                &:first-child{
                    height: 30px;
                }

                li{

                    margin-bottom: 36px;
                    h4{
                        font-size: 25px;
                    }

                    .light-grey{
                        color: lightgray;
                    }

                }

                .course{
                    font-size: 18px;
                    color: lightgrey;
                }

                .box-img{
                    width: 100%;
                    img{
                        width: 100%;
                    }
                }
            }

            .col-2,
            .col-3{
                li{
                    &:hover .course,
                    &:hover{
                        color: #40C4FF;
                    }
                    &:hover:first-child{
                        color: white;
                    }
                }
            }
        }
        .copy{
            line-height: 50px;
        }
    }   
}
</style>