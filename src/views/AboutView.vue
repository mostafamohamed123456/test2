<template>
    <div class="about-page">
        <LeftNav />
        <profile />
        <chat />
        <contact />
    </div>
</template>
<script>
    import LeftNav from "../components/AboutLeft.vue";
    import profile from "../components/AboutProfile.vue";
    import chat from "../components/AboutChat.vue";
    import contact from "../components/AboutContact.vue";
    export default {
        name:"about",
        components:{
            LeftNav,
            profile,
            chat,
            contact
        },
        methods:{
            addClassesShowHidden:function(){
                let navBtns = document.querySelectorAll(".left-nav li");
                let aboutItems = document.querySelectorAll(".about-page .directChild");
                navBtns.forEach((navBtn,index)=>{
                    navBtn.addEventListener("click",()=>{
                        //remove class from other btns
                        navBtns.forEach((removeClass)=>removeClass.classList.remove("active"));
                        //add class to current btn
                        navBtn.classList.add("active");
                        //add class active to the directChild
                        if(navBtn.classList.contains("active")){
                            aboutItems.forEach((item)=>{
                                item.classList.remove("active")
                            })
                            aboutItems[index].classList.add("active")
                        }
                        
                    })
                })
            }
        },
        mounted(){
            this.addClassesShowHidden();
        }
    }
</script>
<style lang="scss">
    @import "../components/styles/main.css";
</style>