<script setup>
import { computed, ref } from 'vue';
import Navbar from '../components/Navbar.vue';
import { loadState } from '../utils/Store.js';

const theme = ref(loadState('theme') || 'light')

const mixed = computed(()=>{
  if(theme.value == 'light'){
    return `screen`;
  }
  else return `difference`
})


</script>

<template>
  <div class="">
    <Navbar/>
    <div class="container-flex bg-none overflow-scroll">
      <!-- INTRODUCTION -->
      <section class="row text-center bg-none bdy align-items-center p-5 mx-0">
        <div class="bg-none col-8">
          <h1 class="text-center">Anne Hunt:</h1>
            <h2 class="text-end text-focus-in">developer</h2>
            <h2 class="text-end text-focus-in second">creator</h2>
            <h2 class="text-end text-focus-in third">problem-solver</h2>
            <h2 class="text-end text-focus-in fourth">mystery</h2>
        </div>
      </section>
      <!--SHOW OFF-->
      <section class="row bg-page">
        <div class="col-4">
          <div class="p-5 jello-horizontal">
            <div id="screencarousel" class="carousel slide carousel-fade display border">
              <div class="carousel-inner">
                <div class="carousel-item active flicker-1">
                  <img src="../assets/img/display.png" class="d-block w-100" alt="...">
                </div>
                <div class="carousel-item flicker-1">
                  <img src="../assets/img/csharp.png" class="d-block w-100" alt="...">
                </div>
                <div class="carousel-item flicker-1">
                  <img src="../assets/img/vue.png" class="d-block w-100" alt="...">
                </div>
                <div class="carousel-item flicker-1">
                  <img src="../assets/img/mongo.png" class="d-block w-100" alt="...">
                </div>
                <div class="carousel-item flicker-1">
                  <img src="../assets/img/postman.png" class="d-block w-100" alt="...">
                </div>
                <div class="carousel-item flicker-1">
                  <img src="../assets/img/minecraft.png" class="d-block w-100" alt="...">
                </div>
              </div>
            </div>
          </div>
        </div>

        <!--KEYBOARD-->
        <i class="mdi mdi-mouse fs-1" type="button" data-bs-target="#screencarousel" data-bs-slide="next"></i>
      </section>
      <!-- FEATURED PROJECT -->
      <FeaturedProject/>
      <!-- ABOUT ME -->
      <AboutMe/>
      <!-- PORTFOLIO  -->
      <Portfolio/>
      <!-- RESUME -->
      <Resume/>
      <!-- CONTACT -->
      <Contact/>
    </div>
  </div>
</template>

<style scoped lang="scss">
h1, h2, h3, h4, h5{
  font-family: "Kanit", sans-serif;
  font-weight: 700;
  font-style: normal;
}

.display{
  width: 50dvh;
  height: auto;
	-webkit-animation: shadow-pop-tl 0.3s cubic-bezier(0.470, 0.000, 0.745, 0.715) both;
  animation: shadow-pop-tl 0.3s cubic-bezier(0.470, 0.000, 0.745, 0.715) both;
}

.flicker-1 {
	-webkit-animation: flicker-1 2s linear 1s both;
  animation: flicker-1 2s linear 1s both;
}

.jello-horizontal {
	-webkit-animation: jello-horizontal 0.9s both;
  animation: jello-horizontal 0.9s both;
}

 @-webkit-keyframes flicker-1 {
  0%,
  100% {
    opacity: 1;
  }
  41.99% {
    opacity: 1;
  }
  42% {
    opacity: 0;
  }
  43% {
    opacity: 0;
  }
  43.01% {
    opacity: 1;
  }
  47.99% {
    opacity: 1;
  }
  48% {
    opacity: 0;
  }
  49% {
    opacity: 0;
  }
  49.01% {
    opacity: 1;
  }
}
@keyframes flicker-1 {
  0%,
  100% {
    opacity: 1;
  }
  41.99% {
    opacity: 1;
  }
  42% {
    opacity: 0;
  }
  43% {
    opacity: 0;
  }
  43.01% {
    opacity: 1;
  }
  47.99% {
    opacity: 1;
  }
  48% {
    opacity: 0;
  }
  49% {
    opacity: 0;
  }
  49.01% {
    opacity: 1;
  }
}

 @-webkit-keyframes jello-horizontal {
  0% {
    -webkit-transform: scale3d(1, 1, 1);
            transform: scale3d(1, 1, 1);
  }
  30% {
    -webkit-transform: scale3d(1.25, 0.75, 1);
            transform: scale3d(1.25, 0.75, 1);
  }
  40% {
    -webkit-transform: scale3d(0.75, 1.25, 1);
            transform: scale3d(0.75, 1.25, 1);
  }
  50% {
    -webkit-transform: scale3d(1.15, 0.85, 1);
            transform: scale3d(1.15, 0.85, 1);
  }
  65% {
    -webkit-transform: scale3d(0.95, 1.05, 1);
            transform: scale3d(0.95, 1.05, 1);
  }
  75% {
    -webkit-transform: scale3d(1.05, 0.95, 1);
            transform: scale3d(1.05, 0.95, 1);
  }
  100% {
    -webkit-transform: scale3d(1, 1, 1);
            transform: scale3d(1, 1, 1);
  }
}
@keyframes jello-horizontal {
  0% {
    -webkit-transform: scale3d(1, 1, 1);
            transform: scale3d(1, 1, 1);
  }
  30% {
    -webkit-transform: scale3d(1.25, 0.75, 1);
            transform: scale3d(1.25, 0.75, 1);
  }
  40% {
    -webkit-transform: scale3d(0.75, 1.25, 1);
            transform: scale3d(0.75, 1.25, 1);
  }
  50% {
    -webkit-transform: scale3d(1.15, 0.85, 1);
            transform: scale3d(1.15, 0.85, 1);
  }
  65% {
    -webkit-transform: scale3d(0.95, 1.05, 1);
            transform: scale3d(0.95, 1.05, 1);
  }
  75% {
    -webkit-transform: scale3d(1.05, 0.95, 1);
            transform: scale3d(1.05, 0.95, 1);
  }
  100% {
    -webkit-transform: scale3d(1, 1, 1);
            transform: scale3d(1, 1, 1);
  }
}

@-webkit-keyframes shadow-pop-tl {
  0% {
    -webkit-box-shadow: 0 0 #3e3e3e, 0 0 #3e3e3e, 0 0 #3e3e3e, 0 0 #3e3e3e, 0 0 #3e3e3e, 0 0 #3e3e3e, 0 0 #3e3e3e, 0 0 #3e3e3e;
            box-shadow: 0 0 #3e3e3e, 0 0 #3e3e3e, 0 0 #3e3e3e, 0 0 #3e3e3e, 0 0 #3e3e3e, 0 0 #3e3e3e, 0 0 #3e3e3e, 0 0 #3e3e3e;
    -webkit-transform: translateX(0) translateY(0);
            transform: translateX(0) translateY(0);
  }
  100% {
    -webkit-box-shadow: -1px -1px #3e3e3e, -2px -2px #3e3e3e, -3px -3px #3e3e3e, -4px -4px #3e3e3e, -5px -5px #3e3e3e, -6px -6px #3e3e3e, -7px -7px #3e3e3e, -8px -8px #3e3e3e;
            box-shadow: -1px -1px #3e3e3e, -2px -2px #3e3e3e, -3px -3px #3e3e3e, -4px -4px #3e3e3e, -5px -5px #3e3e3e, -6px -6px #3e3e3e, -7px -7px #3e3e3e, -8px -8px #3e3e3e;
    -webkit-transform: translateX(8px) translateY(8px);
            transform: translateX(8px) translateY(8px);
  }
}
@keyframes shadow-pop-tl {
  0% {
    -webkit-box-shadow: 0 0 #3e3e3e, 0 0 #3e3e3e, 0 0 #3e3e3e, 0 0 #3e3e3e, 0 0 #3e3e3e, 0 0 #3e3e3e, 0 0 #3e3e3e, 0 0 #3e3e3e;
            box-shadow: 0 0 #3e3e3e, 0 0 #3e3e3e, 0 0 #3e3e3e, 0 0 #3e3e3e, 0 0 #3e3e3e, 0 0 #3e3e3e, 0 0 #3e3e3e, 0 0 #3e3e3e;
    -webkit-transform: translateX(0) translateY(0);
            transform: translateX(0) translateY(0);
  }
  100% {
    -webkit-box-shadow: -1px -1px #3e3e3e, -2px -2px #3e3e3e, -3px -3px #3e3e3e, -4px -4px #3e3e3e, -5px -5px #3e3e3e, -6px -6px #3e3e3e, -7px -7px #3e3e3e, -8px -8px #3e3e3e;
            box-shadow: -1px -1px #3e3e3e, -2px -2px #3e3e3e, -3px -3px #3e3e3e, -4px -4px #3e3e3e, -5px -5px #3e3e3e, -6px -6px #3e3e3e, -7px -7px #3e3e3e, -8px -8px #3e3e3e;
    -webkit-transform: translateX(8px) translateY(8px);
            transform: translateX(8px) translateY(8px);
  }
}

.text-focus-in {
	-webkit-animation: text-focus-in 1s cubic-bezier(0.550, 0.085, 0.680, 0.530) both;
    animation: text-focus-in 1s cubic-bezier(0.550, 0.085, 0.680, 0.530) both;
}

.text-focus-in.second {
	-webkit-animation: text-focus-in 1s cubic-bezier(0.550, 0.085, 0.680, 0.530) 1s both;
    animation: text-focus-in 1s cubic-bezier(0.550, 0.085, 0.680, 0.530) 1s both;
}

.text-focus-in.third {
	-webkit-animation: text-focus-in 1s cubic-bezier(0.550, 0.085, 0.680, 0.530) 2s both;
    animation: text-focus-in 1s cubic-bezier(0.550, 0.085, 0.680, 0.530) 2s both;
}

.text-focus-in.fourth {
	-webkit-animation: text-focus-in 1s cubic-bezier(0.550, 0.085, 0.680, 0.530) 3s both;
    animation: text-focus-in 1s cubic-bezier(0.550, 0.085, 0.680, 0.530) 3s both;
}

 @-webkit-keyframes text-focus-in {
  0% {
    -webkit-filter: blur(12px);
            filter: blur(12px);
    opacity: 0;
  }
  100% {
    -webkit-filter: blur(0px);
            filter: blur(0px);
    opacity: 1;
  }
}
@keyframes text-focus-in {
  0% {
    -webkit-filter: blur(12px);
            filter: blur(12px);
    opacity: 0;
  }
  100% {
    -webkit-filter: blur(0px);
            filter: blur(0px);
    opacity: 1;
  }
}

.codeworks{
  color: rgb(48,164,218);
}

.uwm{
  color: rgb(255, 194, 47);
}

.uwyo{
  color: rgb(73, 47, 37);
}

.bhsu{
  color: rgb(0, 98, 54)
}

.bg{
  background-color: black;
  background-image: linear-gradient( 76.9deg,  rgba(255,90,90,1) 27.2%, rgba(130,5,255,1) 79.9% );
  height: auto;
}

.bdy{
  height: auto;
  mix-blend-mode: screen;
  background-color: var(--bs-page);
  color: black;
  font-size: 10vw; /* Responsive font size */
  font-weight: bold;
  text-shadow: black;
  font-family: Asap, Verdana, Geneva, Tahoma, sans-serif;
}

.bg-page{
  background-color: var(--bs-page);
}

.screen{
  mix-blend-mode: screen;
  background-color: var(--bs-page);
  color: black;
  font-weight: bold;
  text-shadow: black;
}

.featured{
  background-image: url('https://images.unsplash.com/photo-1627308594190-a057cd4bfac8?w=900&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8MzF8fHNtb290aGllfGVufDB8fDB8fHww');
  background-color: black;
  background-position: center;
  background-size: cover;
  min-width: 50dvh;
  min-height: 50dvh;
}

.profile{
  height: 30dvh;
  width: 30dvh;
  object-fit: cover;
  object-position: center;
}

.ukey1{
  min-width: 6%;
}

.ukey15{
  min-width: 10%;
}

.ukey2{
  min-width: 13.32%;
}


</style>
