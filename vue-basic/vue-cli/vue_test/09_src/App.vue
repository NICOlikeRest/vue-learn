<template>
  <div class="app">
    <div v-text="msg"></div>
    <!-- <StudentCom v-on:atguigu="demo"></StudentCom> -->
    <SchoolCom :getSchoolName="getSchoolName"></SchoolCom>
    <StudentCom ref="student"></StudentCom>

  </div>
</template>

<script>
import StudentCom from './components/StudentCom.vue'
import SchoolCom from './components/SchoolCom.vue'
export default {
    name: 'App',
    components:{StudentCom,SchoolCom},
    data() {
      return {
        msg: "hello"
      }
    },
    methods:{
      getSchoolName(name) {
        console.log('App收到了学校名：', name);
      },
      demo(name){
        // console.log('demo被调用了');
        console.log('App收到了学生名：', name);

      }
    },
    mounted(){
      this.$refs.student.$on('atguigu', this.demo)
    }

}
</script>

<style scoped>
  .app {
    background-color: pink;
  }
</style>