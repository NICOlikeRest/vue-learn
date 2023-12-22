<template>
  <div>
    <button @click="getStudents">获取学术信息</button>
  </div>
</template>

<script>
import axios from 'axios'
export default {
  name: "App",
  methods:{
    getStudents() {
      axios.get('http://localhost:8080/api/students').then(
        response => {
          console.log('请求成功了', response.data);
        },
        error => {
          console.log('err', err);
        }
      )
    }
  }
  
  
}
</script>

<style>
  

</style>