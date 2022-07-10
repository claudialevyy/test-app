<template>
  <div>
    <HelloWorld/>
    <UserInformation/>
    <Counter/>
    <Form/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import UserInformation from "@/components/UserInformation";
import Counter from "@/components/Counter";
import Form from "@/components/Form";

export default {
  name: 'App',
  components: {
    HelloWorld,
    UserInformation,
    Counter,
    Form
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
