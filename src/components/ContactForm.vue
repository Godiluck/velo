<template>
  <div class="wrapper">
    <div class="form">
      <h2>Drop your contacts here, pal!</h2>
      <form>
        <input type="text" placeholder="Your name">
        <input type="tel" placeholder="Phone number">
        <input type="text" placeholder="Your question or comment (unnecessary)">
        <input type="submit" value="Send request">
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: "ContactForm",
  props: {
    visible: Boolean,
  }
}
</script>

<style scoped>

</style>