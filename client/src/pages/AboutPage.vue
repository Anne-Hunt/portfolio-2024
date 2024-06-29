<script setup>

</script>

<template>
<section class="row fill px-4 m-0 py-0 bg-page justify-content-center align-items-top">
  <div class="row align-items-center justify-content-evenly">

    <div class="col px-0">
      <About/>
    </div>
    <div class="col p-0">
      <div class="row">
        <div class="col-12 p-0 m-0 d-flex justify-content-center">
          <img src="https://i.imgur.com/OVw48yL.png" alt="Face of Anne Hunt">
        </div>
        <div class="col-12 text-center p-0 m-0">
          <h3>A face you can trust!</h3>
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
.bg-page{
  background-color: var(--bs-page);
}
.bg{
  background-color: black;
  background-image: linear-gradient( 76.9deg,  rgba(255,90,90,1) 27.2%, rgba(130,5,255,1) 79.9% );
  height: auto;
}

.screen{
  mix-blend-mode: screen;
  background-color: var(--bs-page);
  color: black;
  font-weight: bold;
  text-shadow: black;
}

img{
    max-height: 80dvh;
}

.fill{
  height: 100dvh;

}
</style>