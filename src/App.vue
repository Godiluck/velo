<template>
  <PageHeader/>
  <HomePart/>
  <InfoModule/>
</template>

<script>

import PageHeader from "@/components/PageHeader";
import HomePart from "@/components/HomePart";
import InfoModule from "@/components/InfoModule";
export default {
  name: 'App',
  components: {
    InfoModule,
    HomePart,
    PageHeader
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  position: relative;
}
</style>
