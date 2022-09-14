<template>
    <div class="directChild profile active">
        <header class="fixed-header-1">hello,i am mostafa mohamed</header>
        <header class="fixed-header-2">from giza, egypt</header>
        <p class="brief">i'm front-end developer, it's my portfolio website that made by vue.js. you can go to my <button id="projects-website">projects</button> website and checkout my work. </p>
        <div class="graduation">
            <div class="container">
                <img src="../assets/graduation.svg" class="graduation-img">
                <span>graduated from: </span>
            </div>
            <p class="graduation-detail">Higher Institute for Computer Sciences and Information Systems, 6th of October — Bachelor's Degree in Computer Sciences. </p> 
        </div>
        <div class="social">
            <span><i class="fab fa-linkedin"></i></span>
            <span><i class="fab fa-github"></i></span>
            <span><i class="far fa-envelope"></i></span>
            <span><i class="fab fa-facebook-square"></i></span>
        </div>
    </div>
</template>
<script>
    export default {
        name:"profile",
        methods:{
            projectsWebsite:function(){
                let projectBtn = document.getElementById("projects-website");
                let projectLink = document.querySelector(".navBar-list li a[href='/projects']");
                projectBtn.onclick = ()=>{
                    projectLink.click();
                }
            }
        },
        mounted(){
            this.projectsWebsite();
        }
    }
</script>
<style lang="scss"></style>