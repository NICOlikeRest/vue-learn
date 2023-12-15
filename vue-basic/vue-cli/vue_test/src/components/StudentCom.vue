<template>
  <div>
    <div v-text='msg'></div> <hr>
    学生名称：{{name}}  <hr>
    学生性别：{{sex}} <hr>
    学生年龄：{{age+1}} <hr>
  </div>
</template>

<script>
export default {
    name: 'SchoolCom',
    data() {
        return {
            msg: 'hello'
        }
    },
    // props:['name', 'age', 'sex']
    props: {
      name:String,
      age:Number,
      sex:String
    }
}
</script>

<style>

</style>