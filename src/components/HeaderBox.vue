<template>
    <header>
        <header-content
        :content="contentList[currentContent]"/>
        <div class="register-button">Register Now</div>
        <div class="select-box">
            <div v-for="(el, index) in contentList" 
            :key="index"
            @click="setCurrentContent(index)"></div>
        </div>
    </header>
</template>

<script>
import HeaderContent from './HeaderContent.vue'
export default {
    components: { 
        HeaderContent 
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
header{
    height: 100vh;
    width: 100%;
    position: relative;

    .register-button{
        z-index: 1;
        position:absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%,-50%);
        margin-top: 120px;
    }

    .select-box{
        z-index: 1;
        position:absolute;
        bottom:0;
        left: 50%;
        transform: translate(-50%, 0);
        height: 40px;
        display: flex;
        div{
            margin: 12px;
            width: 20px;
            height: 20px;
            border-radius: 100%;
            border: black solid 1px;
            
            //transform: translate(-50%, 0);
        }
    }
}

</style>