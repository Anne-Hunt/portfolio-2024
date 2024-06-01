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
            <h2 class="text-end text-focus-in fourth">developer</h2>
        </div>
      </section>
      <!-- FEATURED PROJECT -->
      <section class="row bg-none justify-content-center mx-0">
        <div class="screen p-3"><h3 class="text-center">
          FEATURED WORK
        </h3>
      </div>
       <div class="row bg-page py-5 justify-content-center">

         <div class="col-md-4 col-12 order-1 featured">

         </div>
         <div class="col-md-4 col-12 order-2 bg-page border p-3">
           <h3>All Spice</h3>
           <div>
             All Spice is a comprehensive solution to keeping and sharing recipes without having to scroll through the creator's entire life history with specific ingredients or memories of cookies past.
           </div>
           <div>
             Backend: SQL, C#, .NET || Frontend: Javascript, Bootstrap 5, Vue.js 3, HTML, CSS 
           </div>
           <div class="bg-none text-end"><i class="mdi mdi-arrow-up-right-bold fs-3 btn "></i></div>
         </div>
       </div>
      </section>
      <!-- ABOUT ME -->
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
      <!-- PORTFOLIO  -->
      <section class="row bg-none justify-content-center mx-0">
        <div class="screen p-3"><h3 class="text-center">
          PORTFOLIO
        </h3>
      </div>
       <div class="row bg-page py-5 justify-content-center">
        <div class="col-md-5 col-12 mb-2">
          <div class="bg-dark opacity-25 rounded p-2">
            <h5 class="opacity-100 text-white">
              Keepr
            </h5>
            <p class="opacity-100 text-white">description</p>
            <p class="opacity-100 text-white text-end m-0">see the code <a href="https://github.com/Anne-Hunt/keepr"><i class="mdi mdi-code-block-tags"></i></a> or live site <a href=""><i class="mdi mdi-application-brackets-outline"></i></a></p>
          </div>
        </div>
        <div class="col-md-5 col-12 mb-2">
          <div class="bg-dark opacity-25 rounded p-2">
            <h5 class="opacity-100 text-white">
              Spuditions
            </h5>
            <p class="opacity-100 text-white">description</p>
            <p class="opacity-100 text-white text-end m-0">see the code <a href="https://github.com/Anne-Hunt/spuditions"><i class="mdi mdi-code-block-tags"></i></a> or live site <a href=""><i class="mdi mdi-application-brackets-outline"></i></a></p>
          </div>
        </div>
        <div class="col-md-5 col-12 mb-2">
          <div class="bg-dark opacity-25 rounded p-2">
            <h5 class="opacity-100 text-white">
              Swarm
            </h5>
            <p class="opacity-100 text-white">description</p>
            <p class="opacity-100 text-white text-end m-0">see the code <a href="https://github.com/Anne-Hunt/Swarm"><i class="mdi mdi-code-block-tags"></i></a> or live site <a href=""><i class="mdi mdi-application-brackets-outline"></i></a></p>
          </div>
        </div>
        <div class="col-md-5 col-12 mb-2">
          <div class="bg-dark opacity-25 rounded p-2">
            <h5 class="opacity-100 text-white">
              The Codework
            </h5>
            <p class="opacity-100 text-white">description</p>
            <p class="opacity-100 text-white text-end m-0">see the code <a href="https://github.com/Anne-Hunt/The-Codework"><i class="mdi mdi-code-block-tags"></i></a> or live site <a href=""><i class="mdi mdi-application-brackets-outline"></i></a></p>
          </div>
        </div>
         
       </div>
      </section>
      <!-- RESUME -->
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
       </div>
       <h4 class="text-center m-0 bg-page p-3">WORK</h4>
       <div class="row justify-content-center text-start m-0 p-0">
          <div class="row screen m-0">
            <h5 class="px-5">Full Stack Web Developer</h5>
          </div>
          <div class="row m-0 bg-page px-5">
            <p><strong>Boise CodeWorks</strong></p>
            <p class="px-5">Created and developed website applications according to requirements, including Figma models, UML and database requirements, and Scrum/Agile best practices, both as an individual and as a member of a team.</p>
          </div>
          <div class="row screen m-0">
            <h5 class="px-5">Digital Marketing</h5>
          </div>
          <div class="row bg-page m-0 px-5">
            <p><strong>Quick Wit Marketing</strong></p>
            <p class="px-5">Maintaining online marketing presences for local businesses, content creation, basic web development, project management, event coordination</p>
          </div>
          <div class="row screen">
            <h5 class="px-5">Marketing Manager</h5>
          </div>
          <div class="row bg-page px-5">
            <p><strong>Atlas Resell Management</strong></p>
            <p class="px-5">Data management in a MySql database and adopting new CRM technology, overseeing development of a new website, planning and deploying marketing strategies, process improvement, content creation, management and leadership.</p>
          </div>
          <div class="row screen m-0">
            <h5 class="px-5">English Instructor</h5>
          </div>
          <div class="row bg-page px-5">
            <p><strong>University of Wisconsin-Milwaukee, University of Wyoming</strong></p>
            <p class="px-5">Teaching required English composition courses to students from a diverse range of backgrounds, understanding and employing of pedagogy, digital media use in classroom</p>
          </div>
        </div>
       <h4 class="text-center bg-page m-0 p-3">EDUCATION</h4>
       <div class="row text-center py-3 px-5 bg-page">
        <div class="col-md-3 col-6">
          <i class="mdi mdi-hexagon-multiple-outline fs-1 codeworks"></i>
          <p class="m-0">Boise Codeworks</p>
          <p><small>Graduate</small></p>
        </div>
        <div class="col-md-3 col-6">
          <i class="mdi mdi-paw fs-1 uwm"></i>
          <p class="m-0">University of Wisconsin-Milwaukee</p>
          <p><small>PhD (inc.)</small></p>
        </div>
        <div class="col-md-3 col-6">
          <i class="mdi mdi-account-cowboy-hat fs-1 uwyo"></i>
          <p class="m-0">University of Wyoming</p>
          <p><small>Master of Arts</small></p>
        </div>
        <div class="col-md-3 col-6">
          <i class="mdi mdi-bee fs-1 bhsu"></i>
          <p class="m-0">Black Hills State University</p>
          <p><small>Bachelor of Arts</small></p>
        </div>
       </div>
      </section>
      <!-- CONTACT -->
      <section class="row screen bg-none justify-content-center mx-0">
        <div class="p-2">
          <h3 class="text-center">
          CONTACT ME
        </h3>
      </div>
       <div class="row py-3 justify-content-center">
        <div class="col-4 d-flex justify-content-between">
          <a href="mailto:acathunt@gmail.com"><i class="mdi mdi-email fs-1" role="button"></i></a>  <a href="https://github.com/Anne-Hunt/anne-hunt"><i class="mdi mdi-github fs-1" role="button"></i></a>  <a href="https://www.linkedin.com/in/anne-hunt-developer/"><i class="mdi mdi-linkedin fs-1" role="button"></i></a>
        </div>
       </div>
      </section>
    </div>
  </div>
</template>

<style scoped lang="scss">
h1, h2, h3, h4, h5{
  font-family: "Kanit", sans-serif;
  font-weight: 700;
  font-style: normal;
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
</style>
