<script setup>
import { AppState } from './AppState'
import Navbar from './components/Navbar.vue'


</script>

<template>
    <main class="bg bg-pan-left">
      <router-view />
    </main>
</template>

<style lang="scss">
@import "./assets/scss/main.scss";

:root {
  --main-height: calc(100vh - 32px - 64px);
}

.bg{
  background-color: black;
  background-image: linear-gradient( 76.9deg,  rgba(255,90,90,1) 27.2%, rgba(130,5,255,1) 79.9% );
  height: auto;
}

.bg-pan-left {
	-webkit-animation: bg-pan-left 8s infinite both;
  animation: bg-pan-left 8s infinite both;
}

 @-webkit-keyframes bg-pan-left {
  0% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}
@keyframes bg-pan-left {
  0% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}


footer {
  display: grid;
  place-content: center;
  height: 32px;
}
</style>
