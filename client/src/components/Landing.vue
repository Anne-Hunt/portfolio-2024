<script setup>

</script>


<template>
<section class="row m-0 p-0">
    <div class="col-12 screen match p-0 m-0">
        <div class="row m-0 p-0">
            <h1 class="text-center text-black fw-bold p-0 m-0">Anne Hunt</h1>
            <div class="col-1"></div>
            <div class="col-2 text-start text-secondary text-focus-in second p-0">
                <p class="fs-4">coding</p>
                <p class="fs-4">integrity</p>
                <p class="fs-4">testing</p>
                <p class="fs-4">versatile</p>
                <p class="fs-4">creator</p>
                <p class="fs-4">design</p>
                <p class="fs-4">writing</p>
            </div>
            <div class="col-3 text-start text-danger text-focus-in third p-0">
                <p class="fs-4">Javascript</p>
                <p class="fs-4">full stack</p>
                <p class="fs-4">progress</p>
                <p class="fs-4">MongoDB</p>
                <p class="fs-4">Express</p>
                <p class="fs-4">pivot tables</p>
                <p class="fs-4">RESTful API</p>
            </div>
            <div class="col-2 text-end text-primary text-focus-in p-0">
                <p class="fs-4">C#</p>
                <p class="fs-4">SQL</p>
                <p class="fs-4">.NET</p>
                <p class="fs-4">HTML</p>
                <p class="fs-4">logic</p>
                <p class="fs-4">CSS</p>
                <p class="fs-4">Vue.js</p>
            </div>
            <div class="col-3 text-end text-focus-in fourth p-0">
                <p class="fs-4">developer</p>
                <p class="fs-4">creativity</p>
                <p class="fs-4">critical thinking</p>
                <p class="fs-4">problem solver</p>
                <p class="fs-4">data analysis</p>
                <p class="fs-4">always learning</p>
                <p class="fs-4">process analysis</p>
            </div>
            <div class="col-1"></div>
            <p class="text-center fs-1">now available in 3D</p>
        </div>
    </div>
</section>
<section class="row overlay">
        <img src="../assets/img/3dheadshot.png" alt="" class="head p-0">
</section>
</template>


<style lang="scss" scoped>
.match{
    height: 65dvh;
}

.overlay{
  position: absolute;
  z-index: 1;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

p{
    font-weight: bold;
}

.head{
    max-height: 45dvh;
  object-fit: contain;
}

.text-focus-in {
	-webkit-animation: text-focus-in 1s cubic-bezier(0.550, 0.085, 0.680, 0.530) both;
    animation: text-focus-in 1s cubic-bezier(0.550, 0.085, 0.680, 0.530) both;
    padding: none;
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

.bg-page{
  background-color: var(--bs-page);
}

.screen{
  mix-blend-mode: screen;
  background-color: var(--bs-page);
  color: black;
//   font-weight: bold;
  text-shadow: black;
}
</style>