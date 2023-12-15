<template>
  <div class="demo">
    <h2>{{ Name }}</h2>
    <h2>{{ age }}</h2>
    <button @click="showName">点我提示年龄</button>
  </div>
</template>


<script>
export default {
  name: "StudentCom",
  data() {
    return {
      Name: "尚硅谷",
      age: "18",
    };
  },
  methods: {
    showName() {
      alert(this.age);
    },
  },
};
</script>


<style>
.demo {
  background-color: pink;
}
</style>