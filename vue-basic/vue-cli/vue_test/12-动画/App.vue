<template>
  <div>
    <TestCom/>
      <TestCom2/>
        <TestCom3/>
  </div>
</template>

<script>
import TestCom from "./components/TestCom.vue";
import TestCom2 from "./components/TestCom2.vue";
import TestCom3 from "./components/TestCom3.vue";

export default {
  name: "App",
  components: { TestCom, TestCom2, TestCom3 },
  
}
</script>

<style>
  

</style>