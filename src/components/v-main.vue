<template>
    <div class="bg">
        <Concept></Concept>
        <About></About>
        <Education></Education>
        <Program></Program>
        <Course></Course>
        <Process></Process>
        <Subs></Subs>
        <Footer></Footer>
    </div>
</template>
<script>
import About from '@/components/v-about.vue'
import Concept from '@/components/v-concept.vue'
import Education from '@/components/v-education.vue'
import Program from '@/components/v-program.vue'
import Course from '@/components/v-course.vue'
import Process from '@/components/v-process.vue'
import Subs from '@/components/v-subs.vue'
import Footer from '@/components/v-footer.vue'

export default {
    components: {
        About,
        Concept,
        Education,
        Program,
        Course,
        Process,
        Subs,
        Footer,
    },
    name: 'v-main-wrapper',
}
</script>
<style lang="scss" scoped>
.bg {
    background: rgb(37, 34, 55);
    overflow: hidden;
}
</style>