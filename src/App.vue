<script setup>
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>
  <nav class="navbar bg-dark navbar-dark">
  <div class="container">
    <router-link class="navbar-brand" to="/">
      <img src="@/assets/logo.svg" alt="Logo" width="30" height="24" class="d-inline-block align-text-top">
      PokeApi
    </router-link>
    <div class="m-2">
      <router-link active-class="active" class="btn btn-outline-primary me-2" to="/" >Home</router-link>
      <router-link active-class="active" class="btn btn-outline-primary me-2" to="/pokemons">Pokemons</router-link>
      <router-link active-class="active" class="btn btn-outline-primary" to="/favoritos">Favoritos</router-link>
    </div>
  </div>
</nav>
  
<div class="container text-center">
  <RouterView />
</div>
  
</template>

