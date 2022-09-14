<template>
    <div class="directChild chat">
        <ul class="chat-list">
            <li class="left">
                <img src="../assets/male-user.svg" alt="left-user-svg" title="user-male-ask">
                <span>how can i help you ?</span>
            </li>
            <li class="right">
                <span>i need website!</span>
                <img src="../assets/female-user.svg" alt="left-user-svg" title="user-female-ask">
            </li>
            <li class="left">
                <img src="../assets/male-user.svg" alt="left-user-svg" title="user-male-ask">
                <span>Done. Delivery takes 7 Days!</span>
            </li>
        </ul>
        <form class="chat-form">
            <input type="text" placeholder="enter your message" @keyup.enter="this.popUp()">
            <button type="submit"><i class="fab fa-telegram"></i></button>
        </form>
    </div>
</template>
<script>
    export default {
        data(){
            return{
                name: "chat"
            }
        },
        methods:{
            test:function(){
                alert("hello there");
            }
        }
    }
</script>