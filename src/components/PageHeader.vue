<template>
  <div class="wrapper" id="header">
    <div class="logo">
      <img class="logo_inner" src="../assets/baseLogo.png" alt=""/>
    </div>
    <ul class="navbar">
      <li>First point</li>
      <li>Second point</li>
      <li>Third point</li>
    </ul>
  </div>
  <div class="switcher">
    <!--    <img class="header_switcher" id="switcher" src="../assets/arrow.svg" @click="toggleHeader" alt=""/>-->
    <svg @click="toggleHeader" class="header_switcher btn_white" id="switcher" xmlns="http://www.w3.org/2000/svg"
         xmlns:xlink="http://www.w3.org/1999/xlink"
         x="0px" y="0px"
         viewBox="0 0 64 64" xml:space="preserve">
<g id="Up-arrow">
	<path d="M46.7070007,34.2929993c0.3906975,0.3906021,0.3906975,1.0233994,0,1.4140015
		c-0.3906021,0.3906975-1.0233955,0.3906975-1.4140015,0L32,22.4141006L18.7070007,35.7070007
		c-0.3906002,0.3906975-1.0233955,0.3906975-1.4139996,0C17.0977001,35.5116997,17,35.2559013,17,35
		c0-0.2557983,0.0977001-0.5116997,0.2930012-0.7070007l13.9999981-14c0.3906059-0.3906002,1.0233994-0.3906002,1.4140015,0
		L46.7070007,34.2929993z"/>
  <path d="M32,0c-17.6730995,0-32,14.3268995-32,32s14.3268995,32,32,32c17.6731987,0,32-14.3269005,32-32S49.6731987,0,32,0z M32,2
		c16.542099,0,30,13.4580002,30,30c0,16.542099-13.457901,30-30,30s-30-13.457901-30-30C2.0000007,15.4580002,15.4579,2,32,2z"/>
</g>
</svg>
  </div>
</template>

<script>
export default {
  name: "PageHeader",
  methods: {
    toggleHeader() {
      document.getElementById('header').classList.toggle('toggle_header')
      document.getElementById('switcher').classList.toggle('rotate')
      document.getElementById('switcher').classList.toggle('btn_black')
      document.getElementById('switcher').classList.toggle('btn_white')
    },
  }
}
</script>

<style scoped>
.wrapper {
  position: fixed;
  padding-right: 5%;
  width: 95%;
  background: #2c3e50;
  height: 25vh;
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  align-items: center;
  transition: 1s;
  z-index: +1;
}

.toggle_header {
  transform: translateY(-25vh);
  transition: 1s;
}

.rotate {
  transform: rotate(180deg);
  transition: all 1s;
}

.logo {
  width: 15%;
  display: flex;
  height: 100%;
  justify-content: center;
  align-items: center;
}

.logo_inner {
  width: 150px;
  height: auto;
  transition: all .3s;
}

.logo_inner:hover {
  transform: scale(1.2);
  transition: .3s;
}

.navbar {
  height: 30px;
  width: 80%;
  font-family: 'Comfortaa', cursive;
  color: white;
  display: flex;
  flex-direction: row;
  list-style-type: none;
  justify-content: space-evenly;
  font-size: 30px;
}

.navbar > li {
  transition: all .2s;
  cursor: pointer;
}

.navbar > li:hover {
  color: cornflowerblue;
  transition: .2s;
}

.switcher {
  position: fixed;
  top: 0;
  right: 10px;
  height: 25vh;
  display: flex;
  align-items: center;
  z-index: +2;
}

.header_switcher {
  height: 60px;
  margin-right: 20px;
  transition: all 1s;
}

.btn_white {
  fill: white;
}

.btn_black {
  filter: invert(0%) sepia(0%) saturate(0%) hue-rotate(92deg) brightness(98%) contrast(105%);
}

.header_switcher:hover {
  filter: invert(52%) sepia(98%) saturate(1229%) hue-rotate(195deg) brightness(97%) contrast(91%);
  transition: .3s;
}
</style>