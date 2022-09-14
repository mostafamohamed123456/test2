<template>
    <div class="main-home">
        <h1 id="hello-msg"></h1>
        <p class="introduce-msg"></p>
        <p class="introduce-two-msg"></p>
        <a href="mostafa mohamed.pdf" download>download cv <i class="fas fa-download"></i></a>
        <div class="container-one">
            <img src="../assets/01.jpg" class="right-img">
            <div class="after-hovering-img">
                <div class="insider">
                    <span><img alt="idea" src="../assets/idea.svg" width="80" height="80"> <span class="ideas">new ideas</span></span>
                    <span><img alt="happy" src="../assets/happy.svg" width="60" height="60"><span class="users-happy">users happy</span></span>
                    <span><img alt="deadline" src="../assets/deadline.svg" width="60" height="60"><span class="deadline">deadLine</span></span>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
    export default {
        name: "MainHome",
        data(){
            return{
                name:"mainHome",
            }
        },
    }
</script>
<style lang="scss"></style>