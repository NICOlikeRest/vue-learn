<template>
  <div class="test">
    学生名称：{{name}} <hr>
    学生性别：{{sex}} <hr>
    <button @click="sendStudentName">把学生名给school</button>
  </div>
</template>

<script>
export default {
    name: 'StuedntCom',
    data() {
        return {
            name:'yty',
            sex:'male'
        }
    },
    methods:{
      sendStudentName(){
        this.$bus.$emit('hello', 666)
      }
    }


}
</script>

<style lang="less" scoped>
  .test {
    background-color: orange;

  }
</style>