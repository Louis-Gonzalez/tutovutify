<template>
  <div class="navbar">
    <NuxtLink class="item-navbar" to="/" exact-active-class="active-link">Home</NuxtLink>
    <NuxtLink class="item-navbar" to="/about" exact-active-class="active-link">About</NuxtLink>
    <NuxtLink class="item-navbar" to="/contact" exact-active-class="active-link">Contact</NuxtLink>
  </div>
  <div class="current-page">
    <p>Vous êtes sur la page : {{ route.path }}</p>
  </div>
</template>

<script setup lang="ts">
import { useRoute } from 'vue-router';
const route = useRoute();
</script>

<style>
.navbar {
  background-color: black;
  display: flex;
  justify-content: flex-start;
  align-items: center;
  gap: 1rem;
  padding: 0.75rem;
}

.item-navbar {
  color: whitesmoke;
  text-decoration: none;
  font-size: 1rem;
  padding: 0.5rem 0.75rem;
  border-radius: 0.25rem;
  transition: all 0.3s ease;
}

.active-link {
  background-color: red;
  color: whitesmoke !important;
  border: 2px solid whitesmoke;
  font-weight: bold;
  padding: 0.5rem 0.75rem;
  border-radius: 0.25rem;
}

.current-page {
  background-color: #001f3f;
  color: whitesmoke;
  padding: 0.75rem;
  margin-top: 0.75rem;
  border-radius: 0.25rem;
  text-align: center;
}
</style>
