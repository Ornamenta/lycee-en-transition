<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <header>
    <img
      alt="Vue logo"
      class="logo"
      src="@/assets/logo.svg"
      width="125"
      height="125"
    />

    <div class="wrapper">
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>
  <RouterView />
</template>

<style scoped lang="scss">
nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a {
  color: var(--dt-c-on-background);
}
nav a.router-link-exact-active {
  color: var(--dt-c-secondary);
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--dt-c-on-background);
}

nav a:first-of-type {
  border: 0;
}
</style>
