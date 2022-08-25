<template>
  <PageHeader/>
  <HomePart/>
  <InfoModule/>
  <ContactForm/>
</template>

<script>

import PageHeader from "@/components/PageHeader";
import HomePart from "@/components/HomePart";
import InfoModule from "@/components/InfoModule";
import ContactForm from "@/components/ContactForm";
export default {
  name: 'App',
  components: {
    ContactForm,
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
  font-family: 'Comfortaa', cursive;
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
