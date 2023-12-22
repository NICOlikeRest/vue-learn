<template>
  <div class="test">
    学校名称：{{name}}  <hr>
    学校地址：{{address}}

  </div>
</template>

<script>
export default {
    name: 'SchoolCom',
    data() {
        return {
            name: 'shangguigu',
            address: 'hangzhou'
        }
    },
    mounted(){
      // console.log(this.x);
      this.$bus.$on('hello', (data)=>{
        console.log('woshi school', data);
      })
    }
    
}
</script>

<style scoped>
  .test {
    background-color: green;
  }
</style>