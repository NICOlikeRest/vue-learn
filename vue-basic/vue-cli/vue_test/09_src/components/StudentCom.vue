<template>
  <div class="test">
    学生名称：{{name}} <hr>
    学生性别：{{sex}} <hr>
    <button @click="sendStudentName">点击</button>
    <button @click="unbind">解绑</button>

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
      sendStudentName() {
        this.$emit('atguigu', this.name)
      },
      unbind() {
        this.$off('atguigu')
      }
    }

}
</script>

<style lang="less" scoped>
  .test {
    background-color: orange;

  }
</style>