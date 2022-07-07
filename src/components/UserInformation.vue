<template>
  <section id="assignment">
    <h2>{{ name }}</h2>
    <p>{{ age }}</p>
    <p>{{ age + 5 }}</p>
    <p>Favorite Number: {{ randomNumber }}</p>
    <input :value="name" type="text"/>
    <div>
      <img src="https://i2-prod.mirror.co.uk/incoming/article25609246.ece/ALTERNATES/s1200d/0_PUSS-IN-BOOTS.jpg"/>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      name: "Claudia",
      age: 28,
      randomNumber: Math.random() * 1
    };
  },
  methods: {},
};
</script>
<style scoped>
img {
  width: 200px;
  height: 200px;
  margin-top: 10px;
}
</style>
