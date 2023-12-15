<template>
  <div class="demo">
    <h2>{{ Name }}</h2>
    <h2>{{ address }}</h2>
    <button @click="showName">点我提示学校</button>
  </div>
</template>


<script>
export default {
  name: "SchoolCom",
  data() {
    return {
      Name: "尚硅谷",
      address: "北京昌平",
    };
  },
  methods: {
    showName() {
      alert(this.Name);
    },
  },
};
</script>


<style>
.demo {
  background-color: pink;
}
</style>