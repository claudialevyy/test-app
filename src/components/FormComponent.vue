<template>
  <section>
    <h2>Event Practice</h2>
    <button @click.prevent="alertMessage">Show Alert</button>
    <hr/>
    <input v-model="text"
           type="text"/>
    <p>Input text is: {{ text }}</p>
    <hr/>
    <input :value="confirmedText"
           type="text"
           v-on:keyup.enter="(e) => this.confirmedText = e.target.value"/>
    <p>Confirmed text: is : {{ confirmedText }}</p>
    <button @click="resetInput">Reset text</button>
  </section>
</template>
<script>
export default {
  data() {
    return {
      text: "",
      confirmedText: "",
      showConfirmedText: false
    };
  },
  methods: {
    alertMessage() {
      alert("new message !!!!")
    },
    resetInput() {
      this.text = "";
      this.confirmedText = ""
    }
  },
};
</script>