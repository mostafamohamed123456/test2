<template>
    <div class="directChild contact">
        <header>contact me</header>
        <form @submit.prevent>
            <input type="text" placeholder="enter your fullname" v-model="characters">
            <span class="character-error">field must be only characters</span>
            <input type="email" placeholder="enter your email" v-model="checkEmails">
            <span class="sing-error">field must contain example@mail.com</span>
            <input type="password" placeholder="enter your password" v-model="checkPassword">
            <span class="password-error">password must contain mixed between 10 characters and numbers.</span>
            <button type="submit">submit</button>
        </form>
    </div>
    <form>
        
    </form>
</template>
<script>
    export default {
        name:"contact",
        data(){
            return{
                name:"contact",
                characters:'',
                checkEmails:'',
                checkPassword:''
            }
        },
        computed:{
        },
        watch:{
            characters:function(val){
                // Searching For Numbers To display Error if contain number
                if(val == ''){
                    document.querySelector(".character-error").classList.add("show")
                    document.querySelector(".character-error").innerHTML = "field cannot be empty"
                }else{
                    if(val.search(/[0-9]/g) != -1){
                    document.querySelector(".character-error").classList.add("show")
                    }else{
                        document.querySelector(".character-error").classList.remove("show")
                    }
                }
                
            },
            checkEmails:function(){
                //Search For @ Sign To Accept The Entire Email
                let emails = document.querySelector("input[type='email']").value;
                if(emails == ''){
                    document.querySelector(".sing-error").classList.add("show")
                    document.querySelector(".sing-error").innerHTML = "field cannot be empty"
                }else{
                    if(!emails.includes('@')){
                    document.querySelector(".sing-error").classList.add("show");
                    }else{
                        document.querySelector(".sing-error").classList.remove("show")
                    }
                }
            },
            checkPassword:function(passVal){
                //Check password Field if it's empty
                if(passVal != "" || passVal.length == 10){
                    if(passVal.search(/[0-9]/g) != -1){
                        document.querySelector(".password-error").classList.remove("show")
                    }else{
                        document.querySelector(".password-error").classList.add("show")
                    }
                }else{
                    document.querySelector(".password-error").classList.add("show")
                    document.querySelector(".password-error").innerHTML = "field cannot be empty"
                }
            }
        }
    }
</script>
<style lang="scss"></style>