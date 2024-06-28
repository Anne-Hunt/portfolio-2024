<script setup>

</script>


<template>
      <section class="row p-0 justify-content-center m-0">
       <div class="row justify-content-center">
        <h2>About Me</h2>
        <div class="col-12 order-md-1 order-2">
          <p>
            If I have learned anything in my life, it's how to learn. I'm particularly gifted when it comes to language, whether coding or human communication, as I demonstrated in my coding bootcamp and nearly completing a bachelor's in Spanish in a year. I love solving problems and creating simple, elegant solutions that consider future application plans, not just quick fixes. Creating is what I do—whether I'm knitting a sweater or developing an app.
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