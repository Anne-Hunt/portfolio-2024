<script setup>

</script>


<template>
      <section class="row bg-none justify-content-center mx-0">
        <div class="screen p-3"><h3 class="text-center">
          PORTFOLIO
        </h3>
      </div>
       <div class="row bg-page py-5 justify-content-center">
         <div class="col-md-5 col-12 mb-3">
        <div class="portfolio sample1 rounded d-flex align-items-end">
          <div class="bg-dark opacity-75 rounded-bottom p-2 w-100">
            <h5 class="opacity-100 text-white">
              Keepr
            </h5>
            <p class="opacity-100 text-white">description</p>
            <p class="opacity-100 text-white text-end m-0">see the code <a href="https://github.com/Anne-Hunt/keepr"><i class="mdi mdi-code-block-tags"></i></a> or live site <a href=""><i class="mdi mdi-application-brackets-outline"></i></a></p>
          </div>
        </div>
        </div>
        <div class="col-md-5 col-12 mb-2">
          <div class="portfolio sample2 rounded d-flex align-items-end">
            <div class="bg-dark opacity-75 w-100 rounded p-2">
              <h5 class="opacity-100 text-white">
                Spuditions
              </h5>
              <p class="opacity-100 text-white">description</p>
              <p class="opacity-100 text-white text-end m-0">see the code <a href="https://github.com/Anne-Hunt/spuditions"><i class="mdi mdi-code-block-tags"></i></a> or live site <a href=""><i class="mdi mdi-application-brackets-outline"></i></a></p>
            </div>
          </div>
        </div>
        <div class="col-md-5 col-12 mb-2">
          <div class="portfolio sample3 rounded d-flex align-items-end">
          <div class="bg-dark opacity-75 rounded-bottom p-2 w-100">
            <h5 class="opacity-100 text-white">
              Swarm
            </h5>
            <p class="opacity-100 text-white">description</p>
            <p class="opacity-100 text-white text-end m-0">see the code <a href="https://github.com/Anne-Hunt/Swarm"><i class="mdi mdi-code-block-tags"></i></a> or live site <a href=""><i class="mdi mdi-application-brackets-outline"></i></a></p>
          </div>
          </div>
        </div>
        <div class="col-md-5 col-12 mb-2">
          <div class="portfolio sample4 rounded d-flex align-items-end">
          <div class="bg-dark opacity-75 rounded-bottom p-2 w-100">
            <h5 class="opacity-100 text-white">
              The Codework
            </h5>
            <p class="opacity-100 text-white">description</p>
            <p class="opacity-100 text-white text-end m-0">see the code <a href="https://github.com/Anne-Hunt/The-Codework"><i class="mdi mdi-code-block-tags"></i></a> or live site <a href=""><i class="mdi mdi-application-brackets-outline"></i></a></p>
          </div>
          </div>
        </div>
         
       </div>
      </section>
</template>


<style scoped lang="scss">
h1, h2, h3, h4, h5{
  font-family: "Kanit", sans-serif;
  font-weight: 700;
  font-style: normal;
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

.sample1{
  background-image: url('../assets/img/keepr.png');
}

.sample2{
  background-image: url('../assets/img/spuditions.png');
}

.sample3{
  background-image: url('../assets/img/swarm.png');
}

.sample4{
  background-image: url('../assets/img/codework.png');
}

.portfolio{
  background-color: black;
  background-position: center;
  background-size: cover;
  min-width: 50dvh;
  min-height: 50dvh;
}
</style>