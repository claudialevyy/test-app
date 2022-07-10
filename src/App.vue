<template>
  <div>
    <!--    <HelloWorld/>
        <UserInformation/>
        <CounterComponent/>
        <FormComponent/>
        <ActionReactivity/>-->
    <ClassBinding/>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import UserInformation from "@/components/UserInformation";
// import CounterComponent from "@/components/CounterComponent";
// import FormComponent from "@/components/FormComponent";
// import ActionReactivity from "@/components/ActionReactivity";
import ClassBinding from "@/components/ClassBinding";

export default {
  name: 'App',
  components: {
    ClassBinding,
    // ActionReactivity,
    // HelloWorld,
    // UserInformation,
    // CounterComponent,
    // FormComponent
  }
}
</script>

<style>
#app {

}
</style>
