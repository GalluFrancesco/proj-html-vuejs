<template>
    <header>
        <nav-box />
        <header-content
        :content="contentList[currentContent]"/>
        <div class="register-button center-x white txt-base"><B>REGISTER NOW</B></div>
        <div class="select-box center-x">
            <div v-for="(el, index) in contentList" 
            :key="index"
            @click="setCurrentContent(index)"
            class="dot"
            :class="{'border' : currentContent===index}">
            <div v-if="currentContent===index"></div>
            </div>
        </div>
    </header>
</template>

<script>
import HeaderContent from './HeaderContent.vue'
import NavBox from './NavBox.vue';
export default {
    components: { 
        HeaderContent,
        NavBox 
    },
    props:{
        contentList:Array
    },
    data(){
        return{
            currentContent:0
        }
    },
    methods:{
        setCurrentContent(n){
            this.currentContent=n;
        }
    }
    
}
</script>


<style lang="scss" scoped>
@import '../style/variables.scss';

header{
    height: 100vh;
    width: 100%;
    position: relative;
    .register-button{
        bottom: 200px;
        background-color: $main-blue;
        font-size: 12px;
        padding: 22px 40px;
    }

    .select-box{
        display: flex;
        bottom: 0;
        .dot{
            margin:0 12px;
            width: 30px;
            height: 30px;
            border-radius: 100%;
            background-color: rgba(white, 0.3);

            div{
                width: 15px;
                height: 15px;
                background-color: white;
                border-radius: 100%;
                margin: 5px;
            }            //transform: translate(-50%, 0);
        }
        .border{
            border: white solid 3px;
        }
    }
}

</style>