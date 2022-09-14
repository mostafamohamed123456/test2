<template>
    <section class="services">
        <header class="services-header">my <span>services</span></header>
        <div class="container">
            <div>
                <img src="../assets/webdesigner.svg">
                <span>web designer</span>
            </div>
            <div>
                <img src="../assets/webprogrammer.svg">
                <span>web developer</span>
            </div>
            <div>
                <img src="../assets/solvingproblem.svg">
                <span>problem solver </span>
            </div>
            <div>
                <img src="../assets/uiuxl.png">
                <span>ui/ux</span>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name:'services',
        data(){
            return{
                name:'skillsService',
                helloMsg:"hello!,",
                introduceMsg:"my name is mostafa mohamed,",
                introduceTwoMsg:"i'm front-end web development.",
                timing: 100
            }
        },
        methods:{
            
        },
    }
</script>

<style lang="scss" scoped></style>