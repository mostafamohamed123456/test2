<template>
  <div>
    <NavHeader />
  </div>
  <router-view />
</template>
<script>
  import NavHeader from "./components/Header.vue";
  export default {
    name:"App",
    components:{
      NavHeader
    }
  }
</script>

<style lang="scss">
*{
  padding:0;
  margin:0;
  font-family:Arial, sans-serif;
}
</style>
