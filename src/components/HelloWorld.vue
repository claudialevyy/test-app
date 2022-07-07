<template>
  <div>
    <div>
      <label for="goal">Goal </label>
      <input id="goal" v-model="enteredValue" type="text"/>
      <button @click="addGoal">Add Goal</button>
    </div>
    <ul>
      <li v-for="goal in goals" :key="goal">{{ goal }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      goals: [],
      enteredValue: "",
    };
  },
  methods: {
    addGoal() {
      this.goals.push(this.enteredValue);
    },
  },
};
</script>

<style scoped>
li {
  text-align: left;
}
</style>
