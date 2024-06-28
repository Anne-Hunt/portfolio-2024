<script setup>

</script>


<template>
<section class="row m-0 p-0">
    <div class="col-md-4 col-6 order-1 text-center p-0 m-0 match">
        <h1 class="text-center text-black fw-bold screen p-0 m-0">Anne Hunt</h1>
        <div class="row justify-content-center bg-page">
            <img src="../assets/img/3dheadshot.png" alt="" class="head antiscreen align-center">
        </div>
        <div class="row screen h-100 justify-content-center">
            <p class="text-center">now available in 3D</p>
        </div>
    </div>
    <div class="col-md-8 col-12 order-2 screen match p-0 m-0">
        <div class="row m-0 p-0">
            <div class="col-2 text-end text-primary text-focus-in p-0">
                <p class="fs-4">C#</p>
                <p class="fs-4">SQL</p>
                <p class="fs-4">.NET</p>
                <p class="fs-4">HTML</p>
                <p class="fs-4">logic</p>
                <p class="fs-4">CSS</p>
                <p class="fs-4">Vue.js</p>
            </div>
            <div class="col-2 text-end text-secondary text-focus-in second p-0">
                <p class="fs-4">coding</p>
                <p class="fs-4">integrity</p>
                <p class="fs-4">testing</p>
                <p class="fs-4">versatile</p>
                <p class="fs-4">creator</p>
                <p class="fs-4">design</p>
                <p class="fs-4">writing</p>
            </div>
            <div class="col-3 text-end text-danger text-focus-in third p-0">
                <p class="fs-4">Javascript</p>
                <p class="fs-4">full stack</p>
                <p class="fs-4">progress</p>
                <p class="fs-4">MongoDB</p>
                <p class="fs-4">Express</p>
                <p class="fs-4">pivot tables</p>
                <p class="fs-4">RESTful API</p>
            </div>
            <div class="col-4 text-end text-focus-in fourth p-0">
                <p class="fs-4">developer</p>
                <p class="fs-4">creativity</p>
                <p class="fs-4">critical thinking</p>
                <p class="fs-4">problem solver</p>
                <p class="fs-4">data analysis</p>
                <p class="fs-4">always learning</p>
                <p class="fs-4">process analysis</p>
            </div>
        </div>
    </div>
</section>
</template>


<style lang="scss" scoped>
.match{
    height: 80dvh;
}

.head{
    max-height: 65dvh;
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