<script setup>
import {ref} from 'vue'
</script>

<template>
  <div>
    <nav class="navbar navbar-expand-lg navbar-dark custom-navbar">
      <div class="container-fluid">
        <router-link class="navbar-brand" to="/">Full-Time</router-link>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav me-auto">
            <li class="nav-item">
              <router-link class="nav-link" aria-current="page" to="/about"><i class="bi bi-person-add"></i> Novo Motorista</router-link>
            </li>
            <li class="nav-item">
              <router-link class="nav-link" to="/"><i class="bi bi-truck"></i> Roteirizar</router-link>
            </li>
          </ul>
          <ul class="navbar-nav">
            <li class="nav-item">
              <router-link class="nav-link" to="/login"><i class="bi bi-box-arrow-right"></i> Sair</router-link>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </div>
  <div class="main">
    <router-view></router-view>
  </div>
 

 

  
</template>
<style>
.custom-navbar {
  background-color: #ff0000;
}
</style>