<template>
    <main>
        <subjects-box />
        <in-home-tutoring-box />
        <empowering-childre-box />
        <jumbotron-box />
    </main>
</template>

<script>
import EmpoweringChildreBox from './EmpoweringChildreBox.vue'
import InHomeTutoringBox from './InHomeTutoringBox.vue'
import SubjectsBox from './SubjectsBox.vue'
import JumbotronBox from './JumbotronBox.vue'

export default {
    components: { 
        SubjectsBox, 
        InHomeTutoringBox, 
        EmpoweringChildreBox,
        JumbotronBox 
    },
    
}
</script>

<style lang="scss" scoped>

</style>