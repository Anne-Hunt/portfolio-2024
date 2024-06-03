<script setup>

</script>


<template>
      <section class="row bg-none justify-content-center mx-0">
        <div class="screen p-3"><h3 class="text-center">
          ABOUT ME
        </h3>
      </div>
       <div class="row bg-page py-5 justify-content-center">
        <div class="col-md-6 col-12 order-md-1 order-2">
          <p>
            I'm a lifelong creator whose passion is problem solving. Coding is the perfect marriage of language, math, and art. New challenges are an excuse to learn.
          </p>
          <div class="row justify-content-center">
            <div class="col-md-4 col-12">
              <h5>Coding</h5>
              <ul>
                <li>HTML/CSS</li>
                <li>Javascript</li>
                <li>Boostrap 5</li>
                <li>Vue.js 3</li>
                <li>C#</li>
                <li>.NET CORE</li>
              </ul>
            </div>
            <div class="col-md-4 col-12">
              <h5>Working</h5>
              <ul>
                <li>Scrum/Agile</li>
                <li>Problem Solving</li>
                <li>Process Improvement</li>
                <li>Leadership</li>
                <li>Communication</li>
                <li>Organization</li>
              </ul>
            </div>
            <div class="col-md-4 col-12">
              <h5>Creative</h5>
              <ul>
                <li>Knitting</li>
                <li>Book binding</li>
                <li>Baking</li>
                <li>Car Repair</li>
                <li>Woodworking</li>
                <li>Sewing</li>
              </ul>
            </div>
          </div>
        </div>
        <div class="col-4 order-md-2 order-1 d-flex justify-content-center align-items-center">
          <img src="../assets/img/img_face.jpg" alt="Anne Hunt" class="profile border border-2 rounded-circle">
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

.profile{
  height: 30dvh;
  width: 30dvh;
  object-fit: cover;
  object-position: center;
}
</style>