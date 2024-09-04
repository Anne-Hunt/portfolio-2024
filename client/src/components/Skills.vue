<script setup>

</script>


<template>
      <section class="row bg-none justify-content-center mx-0">
        <div class="screen p-3">
          <h3 class="text-center">
          RESUME
        </h3>
      </div>
      <h4 class="text-center bg-page m-0 p-3">SKILLS</h4>
       <div class="row screen py-2 px-5 justify-content-center text-center">
        <div class="text-center col">
          <i class="mdi mdi-dot-net fs-1"></i>
          <p>.NET</p>
        </div>
        <div class="text-center col">
          <i class="mdi mdi-language-csharp fs-1"></i>
          <p>C#</p>
        </div>
        <div class="text-center col">
          <i class="mdi mdi-language-javascript fs-1"></i>
          <p>Javascript</p>
        </div>
        <div class="text-center col">
          <i class="mdi mdi-nodejs fs-1"></i>
          <p>Node.js</p>
        </div>
        <div class="text-center col">
          <i class="mdi mdi-language-html5 fs-1"></i>
          <p>HTML5</p>
        </div>
        <div class="text-center col">
          <i class="mdi mdi-language-css3 fs-1"></i>
          <p>CSS3</p>
        </div>
        <div class="text-center col">
          <i class="mdi mdi-bootstrap fs-1"></i>
          <p>Bootstrap5</p>
        </div>
        <div class="text-center col">
          <i class="mdi mdi-vuejs fs-1"></i>
          <p>Vue.js</p>
        </div>
        <div class="text-center col">
          <i class="mdi mdi-react fs-1"></i>
          <p>React</p>
        </div>
        <div class="text-center col">
          <i class="mdi mdi-tailwind fs-1"></i>
          <p>Tailwind CSS</p>
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

</style>