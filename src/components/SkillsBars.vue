<template>
    <div class="container">
        <div class="html-container ">
            <label><i class="fab fa-html5"></i> html</label>
            <div class="progress-container parent-1">
                <span class="progress-parent"></span>
                <span class="progress-child"></span>
            </div>
        </div>
        <div class="css-container ">
            <label><i class="fab fa-css3-alt"></i> css</label>
            <div class="progress-container parent-2">
                <span class="progress-parent"></span>
                <span class="progress-child"></span>
            </div>
        </div>
        <div class="js-container ">
            <label><i class="fab fa-js"></i> javascript</label>
            <div class="progress-container parent-3">
                <span class="progress-parent"></span>
                <span class="progress-child"></span>
            </div>
        </div>
        <div class="sass-container ">
            <label><i class="fab fa-sass"></i> sass</label>
            <div class="progress-container parent-4">
                <span class="progress-parent"></span>
                <span class="progress-child"></span>
            </div>
        </div>
        <div class="vue-container ">
            <label><i class="fab fa-vuejs"></i> vue.js</label>
            <div class="progress-container parent-5">
                <span class="progress-parent"></span>
                <span class="progress-child"></span>
            </div>
        </div>
        <services />
    </div>
</template>
<script>
    import services from "./SkillsServices.vue"
    export default {
        name: "skillProgressBars",
        components:{
            services
        }
    }
</script>
<style lang="scss"></style>