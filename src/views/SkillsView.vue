<template>
    <div class="skills-page">
        <header class="skills-header">my <span>skills</span></header>
        <SkillsBars />
    </div>
</template>
<script>
    import SkillsBars from '@/components/SkillsBars.vue';
    export default {
        name:"SkillsView",
        data(){
            return{
                name:"skills"
            }
            
        },
        components:{
            SkillsBars
        }
    }
</script>
<style lang="scss">
    @import "../components/styles/main.css";
</style>