<template>
  <div class="test">
    <div v-text='msg' class="qew"></div> <hr>
    学生名称：{{name}} <hr>
    学生性别：{{sex}} <hr>

  </div>
</template>

<script>
export default {
    name: 'SchoolCom',
    data() {
        return {
            msg: 'hello',
            name:'yty',
            sex:'male'
        }
    },

}
</script>

<style lang="less">
  .test {
    background-color: orange;
    .qew{
      font-size: 80px;
    }
  }
</style>