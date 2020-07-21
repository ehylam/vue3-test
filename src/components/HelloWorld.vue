<template>
  <section>
    <h1>{{ msg }}</h1>
    <button @click="count++">count is: {{ count }}</button>
    <p>I'm a {{name}}</p>
    <input type="text" v-model="name" />
    <div class="sub-section">
      <button-comp></button-comp>
    </div>
  </section>
</template>

<script>
import { ref } from "vue";
// Creating usable components within a component.

// const app = createApp({});

// app.component("button-comp", {
//   data() {
//     return {
//       name: "Hello, I'm a button"
//     };
//   },
//   template: `
//     <button>
//       {{name}}
//     </button>
//   `
// });

// app.mount(".sub-section");

export default {
  setup() {},
  props: {
    msg: String,
    name: String
  },
  data() {
    return {
      name: "",
      count: 0
    };
  }
};
</script>
