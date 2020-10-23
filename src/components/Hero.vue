<template>
<b-container fluid class="bv-example-row bv-example-row-flex-cols">
  <br>
  <br>
  <br>
  <br>
  <b-row align-v="center" class="subtext white text-center">
    <div>
      <h2 class="text">YOU CAN’T BUY</h2>
      <h1 class="big-text">HAPPINESS,</h1>
      <h2 class="text">BUT YOU CAN BUY,</h2>
      <h1 class="big-text">CUPCAKES,</h1>
      <h2 class="text">...AND THAT’S KIND </h2>
      <h2 class="text">OF THE SAME THING!</h2>
    </div>
  </b-row>
    <br>
  <br>
  <b-row align-v="center" class="subtext text-center">
    <b-button variant="dark_hue" size="lg">SHOP CUPCAKES</b-button>
  </b-row>
</b-container>
</template>

<script>
export default {
  name: 'Hero'
}
</script>

<style scoped>
.bv-example-row {
  height: 100vh;
  background-image: url("../assets/cup.jpg");
  background-size: cover;
  margin: 0;
  color: white;
  max-width: 100vw;
}
.white {
  background-color: black;
  opacity: 0.7;
}
.subtext {
  display: flex;
  align-content: center;
  justify-content: center;
  margin: 0 200px 0 200px;
}
.text {
  font-weight: 500;
}
.big-text {
  font-weight: 700;
}

@media screen and (max-width: 375px) {
  .subtext {
    margin: 0 20px 0 20px;
  }
}
@media screen and (max-width: 768px) {
  .subtext {
    margin: 0 50px 0 50px;
  }
}

</style>

