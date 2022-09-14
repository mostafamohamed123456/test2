<template>
    <nav>
        <h2>portfolio</h2>
        <ul class="navBar-list">
            <li><router-link to="/" exact><i class="fas fa-home"></i>home</router-link></li>
            <li><router-link to="/about"><i class="fas fa-id-card"></i>about</router-link></li>
            <li><router-link to="/skills"><i class="fas fa-code"></i>skills</router-link></li>
            <li><router-link to="/projects"><i class="fas fa-laptop-code"></i>projects</router-link></li>
        </ul>
    </nav>
</template>
<script>
    export default {
        name:"Header",
    }
</script>
<style lang="scss"></style>