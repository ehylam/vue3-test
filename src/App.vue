<template>
  <section class="home">
    <img alt="Vue logo" src="./assets/logo.png" />
    <Hero title="Eric Lam" />
    <HelloWorld msg="Hello Vue 3.0 + Vite" />
  </section>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import Hero from "./components/Hero.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    Hero
  }
};
</script>
