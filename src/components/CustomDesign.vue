<template>
  <div class="banner">
    <div class="align-center">
      <div class="pt-5 text-center">
        <h1 class="big-text">CUSTOM DESIGN</h1>
        <h2 class="mt-3">YOU DREAM IT, WE CREATE IT</h2>
        <div class="mt-3 pt-5"> <b-link href="#" style="color:white;"><u>VIEW GALLERY</u></b-link></div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'CustomDesign'
}
</script>

<style scoped>
  .banner {
    width: 100vw;
    height: 100vh;
    background: white;
    overflow: hidden;
    }
    .banner .align-center{
      position: relative;
      width: 50vw;
      height: 50vh;
      margin: auto;
      color: white;
      margin-top: 15vh;
      background: var(--dark_hue);
  }
  .big-text {
    font-weight: 700;
  }
  @media screen and (max-width: 768px){
    .banner .align-center{
      position: relative;
      width: 60vw;
      height: 60vh;
      margin: auto;
      color: white;
      margin-top: 5vh;
      background: var(--dark_hue);
  }
  }
</style>

