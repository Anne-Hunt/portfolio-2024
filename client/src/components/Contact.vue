<script setup>

</script>


<template>
      <section class="row screen bg-none justify-content-center mx-0">
        <div class="p-2">
          <h3 class="text-center">
          CONTACT ME!
        </h3>
      </div>
       <div class="row py-3 justify-content-center">
        <div class="col-4 d-flex justify-content-between">
          <i class="mdi mdi-email fs-1" role="button" href="mailto:acathunt@gmail.com"></i>  <i class="mdi mdi-github fs-1" href="https://github.com/Anne-Hunt/anne-hunt" role="button"></i> <i class="mdi mdi-linkedin fs-1" href="https://www.linkedin.com/in/anne-hunt-developer/" role="button"></i>
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

</style>