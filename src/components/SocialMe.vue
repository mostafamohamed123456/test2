<template>
    <div class="social-me">
        <img src="../assets/01.jpg" alt="my-profile-image">
        <span data-link="https://www.linkedin.com/in/mostafa-mohamed-55ab80169/" class="linkedin"><i class="fab fa-linkedin"></i></span>
        <span data-link="https://github.com/mostafamohamed123456" class="github"><i class="fab fa-github"></i></span>
        <span data-link="https://mostafakasper257@gmail.com" class="gmail"><i class="fas fa-envelope"></i></span>
        <span data-link="https://www.facebook.com/mostafa.abosaba" class="facebook"><i class="fab fa-facebook-square"></i></span>
        <span data-link="+201060712125" class="phone"><i class="fas fa-phone-square"></i></span>
    </div>
</template>
<script>
    export default {
        name: "SocialMe",
        methods:{
            mySocialMedia:function(){
                let socialIcons = document.querySelectorAll('.social-me span');
                socialIcons.forEach((icon)=>{
                    icon.addEventListener("click",()=>{
                        if(icon.classList.contains("phone")){
                            return ;
                        }else{
                            window.open(icon.getAttribute("data-link"),"_blank");
                        }
                    })
                })
            }
        },
        mounted(){
            this.mySocialMedia();
        }
    }
</script>
<style lang="scss"></style>