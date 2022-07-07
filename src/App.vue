<template>
  <div>
    <HelloWorld/>
    <UserInformation/>
    <Counter/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import UserInformation from "@/components/UserInformation";
import Counter from "@/components/Counter";

export default {
  name: 'App',
  components: {
    HelloWorld,
    UserInformation,
    Counter
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
