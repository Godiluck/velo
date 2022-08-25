<template>
  <div class="wrapper">
    <div class="card">
      <div class="card-side front">
        <h2 class="header_front">Header Front</h2>
        <p class="body_front">Body Front</p>
      </div>
      <div class="card-side back">
        <h2 class="header_back">Header Back</h2>
        <p class="body_back">Body back</p>
      </div>
    </div>
    <div class="card">
      <div class="card-side front">
        <h2 class="header_front">Header Front</h2>
        <p class="body_front">Body Front</p>
      </div>
      <div class="card-side back">
        <h2 class="header_back">Header Back</h2>
        <p class="body_back">Body back</p>
      </div>
    </div>
    <div class="card">
      <div class="card-side front">
        <h2 class="header_front">Header Front</h2>
        <p class="body_front">Body Front</p>
      </div>
      <div class="card-side back">
        <h2 class="header_back">Header Back</h2>
        <p class="body_back">Body back</p>
      </div>
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
  padding: 10vh 0 10vh 0;
  width: 100%;
  height: 70vh;
//background: white; flex-direction: row;
  display: flex;
  justify-content: space-evenly;
  background: #2c3e50;
}

.card {
  perspective: 150rem;
  position: relative;
  width: 30%;
  max-width: 400px;
  box-shadow: none;
  background: none;
  height: 15vh;
}

.card-side {
  height: 15vh;
  border-radius: 15px;
  transition: all 0.8s ease;
  backface-visibility: hidden;
  position: absolute;
  top: 0;
  left: 0;
  width: 80%;
  padding: 2rem;
  color: white;
}

.card-side.back {
  transform: rotateY(-180deg);
  background-color: #4158D0;
  background-image: linear-gradient(43deg, #4158D0 0%, #C850C0 46%, #FFCC70 100%);
  box-shadow: 5px 5px 9px 0 #80D0C7FF;
}

.card-side.front {
  background-color: #0093E9;
  background-image: linear-gradient(160deg, #0093E9 0%, #80D0C7 100%);
  box-shadow: 5px 5px 9px 0 #C850C0FF;
}

.card:hover .card-side.front {
  transform: rotateY(180deg);
}

.card:hover .card-side.back {
  transform: rotateY(0deg);
}

.header_front{

}

.header_back {

}

.body_front {

}

.body_back {

}
</style>