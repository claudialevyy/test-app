<template>
  <section id="counter">
    <div>{{ counter }}</div>
    <button @click="counter++">+</button>
    <button @click="counter--">-</button>

  </section>
</template>

<script>
export default {
  data() {
    return {
      counter: 0
    };
  },
  methods: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
