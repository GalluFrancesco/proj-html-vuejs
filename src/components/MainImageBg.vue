<template>
    <main>
        <online-courses />
    </main> 
</template>

<script>
import OnlineCourses from './OnlineCourses.vue'
export default {
    components:{
        OnlineCourses
    }
    
}
</script>

<style lang="scss" scoped>
main{
    background: url('/images/page-background-img.png') repeat-y;
    background-size: cover;
}

</style>