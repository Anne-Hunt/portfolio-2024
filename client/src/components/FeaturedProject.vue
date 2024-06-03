<script setup>

</script>


<template>
      <section class="row bg-none justify-content-center mx-0">
        <div class="screen p-3"><h3 class="text-center">
          FEATURED WORK
        </h3>
      </div>
       <div class="row bg-page py-5 justify-content-center">

         <div class="col-md-4 col-12 order-1 featured">

         </div>
         <div class="col-md-4 col-12 order-2 bg-page border p-3">
          <div class="row h-100">
            <div class="align-self-start">
              <h3>All Spice</h3>
              <div>
                All Spice is a comprehensive solution to keeping and sharing recipes without having to scroll through the creator's entire life history with specific ingredients or memories of cookies past.
              </div>
            </div>
            <div class="align-self-end">
              <div>
                Backend: SQL, C#, .NET
              </div>
              <div>
                Frontend: Javascript, Bootstrap 5, Vue.js 3, HTML, CSS 
              </div>
              <div class="bg-none text-end m-0 p-0 text-warning"><i class="mdi mdi-arrow-up-right-bold fs-3 btn m-0 p-0 "></i></div>
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

.featured{
  background-image: url('../assets/img/allspice.png');
  background-color: black;
  background-position: center;
  background-size: cover;
  min-width: 50dvh;
  min-height: 50dvh;
}


</style>