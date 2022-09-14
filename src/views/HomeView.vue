<template>
    <div class="home-page">
        <socialMe />
        <MainHome/>
        <Hoppies />
    </div>
</template>
<script>
    import SocialMe from '@/components/SocialMe.vue';
    import MainHome from '@/components/MainHome.vue';
    import Hoppies from '@/components/Hoppies.vue';
    export default {
        name:"Home",
        components:{
            SocialMe,
            MainHome,
            Hoppies
        },
        data(){
            return{
                
            }
        },
        methods:{
            
        }
    }
</script>
<style lang="scss">
    @import "../components/styles/main.css";
</style>