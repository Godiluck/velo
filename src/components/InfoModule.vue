<template>
  <div class="wrapper">
    <div class="card">
      <div class="card-side front">Text Front</div>
      <div class="card-side back"> Text Back</div>
    </div>
    <div class="card">
      <div class="card-side front">Text Front</div>
      <div class="card-side back"> Text Back</div>
    </div>
    <div class="card">
      <div class="card-side front">Text Front</div>
      <div class="card-side back"> Text Back</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "InfoModule"
}
</script>

<style scoped>
.wrapper {
  background: url("../assets/InfoBack.jpg");
  padding-top: 10vh;
  width: 100%;
  background: white;
  flex-direction: row;
  display: flex;
  justify-content: space-evenly;
}

.card {
  display: none;
  perspective: 150rem;
  position: relative;
  width: 30%;
  max-width: 400px;
  box-shadow: none;
  background: none;
}

.card-side {
  height: 35vh;
  border-radius: 15px;
  transition: all 0.8s ease;
  backface-visibility: hidden;
  position: absolute;
  top: 0;
  left: 0;
  width: 80%;
  padding:2rem;
  color: white
}

.card-side.back {
  transform: rotateY(-180deg);
  background-color: #4158D0;
  background-image: linear-gradient(43deg, #4158D0 0%,#C850C0 46%, #FFCC70 100%);
}

.card-side.front {
  background-color: #0093E9;
  background-image: linear-gradient(160deg, #0093E9 0%, #80D0C7 100%);
}

.card:hover .card-side.front {
  transform: rotateY(180deg);
}

.card:hover .card-side.back {
  transform: rotateY(0deg);
}
</style>