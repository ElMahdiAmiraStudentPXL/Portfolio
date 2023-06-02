<template>
    <div class="navbar">
        <router-link to="/" class="nav-link">Home</router-link>
        <router-link to="/cvview" class="nav-link">CV</router-link>
        <router-link to="/about" class="nav-link">About</router-link>
        <router-link to="/services" class="nav-link">Services</router-link>
        <router-link to="/portfolio" class="nav-link">Portfolio</router-link>
        <router-link to="/contact" class="nav-link">Contact</router-link>
        <a href="https://www.linkedin.com/in/mahdi-amira" class="nav-link">LinkedIn</a>
    </div>
</template>

<style>
.navbar {
    height: 50px;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    background-color: black;
    padding: 10px;
    z-index: 999;
}

.nav-link {
    text-decoration: none;
    color: white;
    display: inline-block;
    padding: 5px 5px;
    transition: background-color 0.3s;

    &:hover {
        background-color: cornflowerblue;
    }
}
</style>

<script setup>
</script>
