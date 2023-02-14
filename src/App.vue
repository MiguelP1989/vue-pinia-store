<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <header class="navbar">
    <div>
      <nav>
        <RouterLink to="/">Posts</RouterLink>
        <RouterLink to="/authors">Authors</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>
.navbar {
  background-color: lightgreen;
  padding: 1.2rem;
}

nav a.router-link-exact-active {
  color: gray;
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid darkgreen;
}

nav a:first-of-type {
  border: 0;
}
</style>
