<template>
    <main>
        <subjects-box />
        <in-home-tutoring-box />
        <empowering-childre-box />
    </main>
</template>

<script>
import EmpoweringChildreBox from './EmpoweringChildreBox.vue'
import InHomeTutoringBox from './InHomeTutoringBox.vue'
import SubjectsBox from './SubjectsBox.vue'


export default {
    components: { 
        SubjectsBox, 
        InHomeTutoringBox, 
        EmpoweringChildreBox 
    },
    
}
</script>

<style lang="scss" scoped>

</style>