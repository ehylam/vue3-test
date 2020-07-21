<template>
  <section class="hero" id="needid">
    <h1>{{title}}</h1>
    <!-- Vue for loop without key.. -->
    <div v-for="text in texts">{{text}}</div>
  </section>
</template>

<script>
export default {
  props: {
    title: String
  },
  data() {
    return {
      texts: ["Hi", "Ho", "No", "Goodbye"]
    };
    // title: "Eric Lam";
  }
};
</script>

<style>
</style>