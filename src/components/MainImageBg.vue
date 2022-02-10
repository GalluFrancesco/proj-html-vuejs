<template>
    <main>
        <online-courses />
        <pricing-box />
    </main> 
</template>

<script>
import OnlineCourses from './OnlineCourses.vue'
import PricingBox from './PricingBox.vue'
export default {
    components:{
        OnlineCourses,
        PricingBox
    }
    
}
</script>

<style lang="scss" scoped>
main{
    background: url('/images/page-background-img.png') repeat-y;
    background-position: 0% 55%;
}

</style>