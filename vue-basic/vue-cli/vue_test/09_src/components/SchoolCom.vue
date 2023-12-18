<template>
  <div class="test">
    学校名称：{{name}}  <hr>
    学校地址：{{address}}
    <button @click="sendSchoolName">点击</button>
  </div>
</template>

<script>
export default {
    name: 'SchoolCom',
    props:['getSchoolName'],    
    data() {
        return {
            name: 'shangguigu',
            address: 'hangzhou'
        }
    },
    methods:{
      sendSchoolName(){
        this.getSchoolName(this.name)
      }
    }

    
}
</script>

<style scoped>
  .test {
    background-color: green;
  }
</style>