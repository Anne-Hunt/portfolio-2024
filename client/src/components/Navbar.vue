<script setup>
import { onMounted, ref } from 'vue';
import { loadState, saveState } from '../utils/Store.js';
import Login from './Login.vue';

const theme = ref(loadState('theme') || 'light')

onMounted(() => {
  document.documentElement.setAttribute('data-bs-theme', theme.value)
})

function toggleTheme() {
  theme.value = theme.value == 'light' ? 'dark' : 'light'
  document.documentElement.setAttribute('data-bs-theme', theme.value)
  saveState('theme', theme.value)
}

</script>

<template>
  <nav class="navbar navbar-expand-sm navbar-dark shadow px-3 bg">
    <router-link class="navbar-brand d-flex" :to="{ name: 'Home' }">
      <div class="d-flex flex-column align-items-center text-light"><strong>HOME</strong>
      </div>
    </router-link>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarText"
      aria-controls="navbarText" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarText">
      <ul class="navbar-nav me-auto">
        <li>
          <router-link :to="{ name: 'About' }" class="btn text-light lighten-30 selectable text-uppercase">
            <strong>ABOUT</strong>
          </router-link>
        </li>
        <li>
          <router-link :to="{ name: 'Resume' }" class="btn text-light lighten-30 selectable text-uppercase">
            <strong>RESUME</strong>
          </router-link>
        </li>
        <li>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle text-light lighten-30 selectable text-uppercase" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            <strong>WORK</strong>
          </a>
          <ul class="dropdown-menu p-2">
            <li><strong>Personal Projects</strong></li>
            <li><a class="dropdown-item" href="https://keepr.annehunt.dev">Keepr</a></li>
            <li><a class="dropdown-item" href="https://allspice.annehunt.dev">AllSpice</a></li>
            <li><a href="https://swarm.annehunt.dev" class="dropdown-item">Swarm</a></li>
            <li><a href="https://jotnotes.annehunt.dev" class="dropdown-item">Jot Notes</a></li>
            <li><hr class="dropdown-divider"></li>
            <li><strong>Team Projects</strong></li>
            <li><a href="https://www.spuditions.com" class="dropdown-item">Spuditions</a></li>
            <li><hr class="dropdown-divider"></li>
            <li>
              <strong>Fun Projects</strong>
            </li>
            <li><router-link :to="{ name: 'Work' }" class="btn selectable">Playground
              </router-link></li>
          </ul>
        </li>
      </ul>
      
      <!-- LOGIN COMPONENT HERE -->
      <!-- <div>
        <button class="btn text-light" @click="toggleTheme"
          :title="`Enable ${theme == 'light' ? 'dark' : 'light'} theme.`">
          <i class="mdi" :class="theme == 'light' ? 'mdi-lightbulb-on' : 'mdi-lightbulb-outline'"></i>
        </button>
      </div> -->
    </div>
  </nav>
</template>

<style scoped>
nav{
  background-image: url(src/assets/img/cubes.png);
}
a:hover {
  text-decoration: none;
}

.nav-link {
  text-transform: uppercase;
}

.navbar-nav .router-link-exact-active {
  border-bottom: 2px solid var(--bs-success);
  border-bottom-left-radius: 0;
  border-bottom-right-radius: 0;
}

.bg{
  background-color: black;
  background-image: linear-gradient( 76.9deg,  rgba(255,90,90,1) 27.2%, rgba(130,5,255,1) 79.9% );
  height: auto;
}

@media screen and (min-width: 576px) {
  nav {
    height: 64px;
  }
}
</style>
