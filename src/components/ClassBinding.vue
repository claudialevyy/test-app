<template>
  <section>
    <!-- 1) Fetch the user input and use it as a CSS class -->
    <!-- The entered class should be added to the below paragraph -->
    <!-- 2) Use the "visible" and "hidden" classes to show/ hide the above paragraph -->
    <div class="container">
      <input v-model="className" type="text"/>
      (available classes: "user1", "user2")
      <button @click="show = !show">Toggle Paragraph</button>
      <p v-show="show" :class="className">
        Style me!
      </p>
    </div>

    <!-- Clicking the button should toggle between the two options -->

    <!-- 3) Add dynamic inline styling to the below paragraph and let the user enter a background-color -->
    <div class="container">
      <input v-model="bgColor" type="text"/>
      <p :style="{'background-color': bgColor }">Style me inline!</p>
    </div>
  </section>
</template>

<script>
export default {
  name: "ClassBinding",
  data() {
    return {
      className: "",
      bgColor: "",
      show: true
    };
  },
  methods: {},
  computed: {}
}
</script>

<style scoped>
.user1 {
  color: red;
}

.user2 {
  color: green;
}

.invisible {
  visibility: hidden;
}

.container {
  width: 400px;
  height: 100px;
}
</style>