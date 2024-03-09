<script setup>
import {RouterLink} from "vue-router";
</script>

<template>
    <header>
        <nav class="container">
            <div class="branding">
                <img src="../assets/Vue_Logo_Black.png" alt="">
                <h1>Vue Todos</h1>
            </div>
            <ul class="nav-routes">
                <RouterLink to="/">Home</RouterLink>
                <RouterLink to="/about">About</RouterLink>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
header {
  background-color: #f1f1f1;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

nav.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 2rem;
}

.branding {
  display: flex;
  align-items: center;
    gap: 8px;
  img {
    margin-right: 15px;
    max-width: 50px;
  }

  h1 {
    color: #333;
    font-size: 24px;
  }
}

.nav-routes {
  display: flex;
  list-style-type: none;

  a {
    display: block;
    padding: 8px 15px;
    text-decoration: none;
    color: #333;
    font-weight: 500;

    &:hover {
      background-color: #e2e2e2;
    }
  }

  a.router-link-exact-active {
    color: #42b983;
  }
}
</style>