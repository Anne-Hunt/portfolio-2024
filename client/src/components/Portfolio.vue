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
            <p class="opacity-100 text-white">Keepr features both private and public content added by users. Both Keeps and Vaults are added allowing users to create saves and then organize links they find helpful, inspirational, or informative.  Keepr uses SQL, C#, .NET, MongoDB, Auth0, Javascript, Vue.js, Bootstrap 5, HTML, CSS, mobile design, and RESTful API design.</p>
            <p class="opacity-100 text-white text-end m-0">see the code <a href="https://github.com/Anne-Hunt/keepr"><i class="mdi mdi-code-block-tags"></i></a> or live site <a href="https://keepr.annehunt.dev"><i class="mdi mdi-application-brackets-outline"></i></a></p>
          </div>
        </div>
        </div>
        <div class="col-md-5 col-12 mb-2">
          <div class="portfolio sample2 rounded d-flex align-items-end">
            <div class="bg-dark opacity-75 w-100 rounded p-2">
              <h5 class="opacity-100 text-white">
                Spuditions
              </h5>
              <p class="opacity-100 text-white">Team work completed in a single week by five talented programmers that allows users to particpate in a forum, view state and national parks in the state of Idaho, and account for the area's specific weather. Spuditions uses Express Node.js, MongoDB, a custom authorization process, Javascript, Vue.js, Bootstrap 5, HTML, CSS, mobile design, MVC, and RESTful API design.</p>
              <p class="opacity-100 text-white text-end m-0">see the code <a href="https://github.com/Anne-Hunt/spuditions"><i class="mdi mdi-code-block-tags"></i></a> or live site <a href="https://www.spuditions.com"><i class="mdi mdi-application-brackets-outline"></i></a></p>
            </div>
          </div>
        </div>
        <div class="col-md-5 col-12 mb-2">
          <div class="portfolio sample3 rounded d-flex align-items-end">
          <div class="bg-dark opacity-75 rounded-bottom p-2 w-100">
            <h5 class="opacity-100 text-white">
              Swarm
            </h5>
            <p class="opacity-100 text-white">Create, edit, and attend events. Users can make comments and view upcoming events. Swarm uses Express Node.js, MongoDB, Auth0, Javascript, Vue.js, Bootstrap 5, HTML, CSS, mobile design, MVC, and RESTful API design.</p>
            <p class="opacity-100 text-white text-end m-0">see the code <a href="https://github.com/Anne-Hunt/Swarm"><i class="mdi mdi-code-block-tags"></i></a> or live site <a href="https://swarm.annehunt.dev"><i class="mdi mdi-application-brackets-outline"></i></a></p>
          </div>
          </div>
        </div>
        <div class="col-md-5 col-12 mb-2">
          <div class="portfolio sample4 rounded d-flex align-items-end">
          <div class="bg-dark opacity-75 rounded-bottom p-2 w-100">
            <h5 class="opacity-100 text-white">
              Jot Notes
            </h5>
            <p class="opacity-100 text-white">Create, edit, and organize notes with Jot. Choose colors, tags, or notebooks for sorting your content and make it private or public. Jot uses Express Node.js, MongoDB, Auth0, Javascript, Vue.js, Bootstrap 5, HTML, CSS, mobile design, MVC, and RESTful API design.</p>
            <p class="opacity-100 text-white text-end m-0">see the code <a href="https://github.com/Anne-Hunt/jot-notes"><i class="mdi mdi-code-block-tags"></i></a> or live site <a href="https://jotnotes.annehunt.dev"><i class="mdi mdi-application-brackets-outline"></i></a></p>
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