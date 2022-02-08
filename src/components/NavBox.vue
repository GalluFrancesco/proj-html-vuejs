<template>
    <nav>
        <div class="logo-box">
            <img src="/images/logo-light.png" alt="">
        </div>
        <ul>
            <li v-for="el in menuElementList"
            :key="el"
            class="txt-base">{{el}}</li>
        </ul>
        <div class="icons-box">
            <i class="fas fa-search"></i>
            <i class="fas fa-shopping-bag">
                <div>0</div>
            </i>
            <i class="fas fa-bars"></i>
        </div>
    </nav>
</template>

<script>
export default {
    data(){
        return{
            menuElementList:['HOME', 'COURSES', 'INSTRUCTORS', 'EVENTS', 'PAGES', 'ELEMENTS']
        }
    }
    
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';
nav{
    width: 100%;
    position: absolute;
    top:36px;
    left:0;
    display: flex;
    align-items: center;
    padding: $main-padding;
    .logo-box{
        width: 300px;
        padding-right: 24px;
        img{
            width: 100%;
        }
    }

    ul{
        padding: 0 24px;
        flex-grow: 1;
        display: flex;
        justify-content: space-between;
        color: white;
        font-size: 18px;
    }

    .icons-box{
        display: flex;
        justify-content: space-between;
        width: 150px;
        color: white;
        font-size: 18px;
        padding-left: 24px;

        .fa-shopping-bag{
            position: relative;
            div{
                position: absolute;
                top: -5px;
                left: 10px;
                width: 20px;
                height: 20px;
                border-radius: 100%;
                background-color: $main-blue;
                text-align: center;
                line-height: 20px;
                font-size: 15px;   
            }
            

        }
    }
}

</style>