<template>
    <main>
        <subjects-box />
        <in-home-tutoring-box />
        <empowering-childre-box />
        <jumbotron-box />
        <learning-box />
        <hr>
    </main>
</template>

<script>
import EmpoweringChildreBox from './EmpoweringChildreBox.vue'
import InHomeTutoringBox from './InHomeTutoringBox.vue'
import SubjectsBox from './SubjectsBox.vue'
import JumbotronBox from './JumbotronBox.vue'
import LearningBox from './LearningBox.vue'

export default {
    components: { 
        SubjectsBox, 
        InHomeTutoringBox, 
        EmpoweringChildreBox,
        JumbotronBox,
        LearningBox 
    },
    
}
</script>

<style lang="scss" scoped>

</style>