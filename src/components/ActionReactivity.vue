<template>
  <section id="assignment">
    <button @click="incrementBy(5)">Add 5</button>
    <button @click="incrementBy(1)">Add 1</button>
    <!-- 1) Connect the buttons and calculate a value (a number) -->
    <!-- Show "Not there yet" until you reach a result of exactly 37 -->
    <!-- Show "Too much!" if the result is greater than 37 -->
    <p>Result: {{ value }}</p>
    <bold>{{ getText }}</bold>
    <!-- 2) Watch for changes in "result" and reset the value to 0 after 5 seconds -->
  </section>
</template>

<script>
export default {
  name: "ActionReactivity",
  data() {
    return {
      value: 0,
      text: ""
    };
  },
  methods: {
    incrementBy(val) {
      this.value += val;
    }
  },
  computed: {
    getText() {
      if (this.value > 37)
        return "Too much!";
      else if (this.value < 37)
        return "Not there yet"
      return "Exact value !!!"
    }
  },
  watch: {
    value() {
      setTimeout(() => {
        this.value = 0;
      }, 3000);
    }
  }

}
</script>

<style scoped>

</style>