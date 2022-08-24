<template>
  <div class="wrapper">
    <div class="text_wrapper">
      <p class="text">Some Greeting Message</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomePart"
}
</script>

<style scoped>
.wrapper {
  background: url("../assets/Kissed-By-the-Paradise-Sun.jpeg");
  height: 100vh;
  width: 100%;
  background-size: auto;
}

.text_wrapper {
  width: 100%;
  position: absolute;
  padding: 60px 0 60px 0;
  top: 60vh;
  background: rgba(0, 0, 0, 0.6);
  backdrop-filter: blur(2px);
  display: flex;
  justify-content: center;
}

.text {
  cursor: default;
  font-size: 30px;
  color: white;
  font-family: 'Comfortaa', cursive;
  border-bottom: 1px solid white;
}
</style>