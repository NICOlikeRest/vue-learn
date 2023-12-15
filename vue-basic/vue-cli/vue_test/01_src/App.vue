<template>
  <div>
    <img src="./assets/logo.png" alt="logo">
    <School></School>
    <Student></Student>
  </div>
</template>

<script>
import School from "./components/SchoolCom.vue";
import Student from "./components/StudentCom.vue";

export default {
  name: "App",
  components: {
    School,
    Student,
  },
};
</script>

<style>
</style>