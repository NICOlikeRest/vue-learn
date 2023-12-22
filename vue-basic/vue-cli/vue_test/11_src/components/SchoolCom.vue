<template>
  <div class="test">
    学校名称：{{name}}  <hr>
    学校地址：{{address}}

  </div>
</template>

<script>
import pubsub from 'pubsub-js'
export default {
    name: 'SchoolCom',
    data() {
        return {
            name: 'shangguigu',
            address: 'hangzhou'
        }
    },
    mounted(){
      // // console.log(this.x);
      // this.$bus.$on('hello', (data)=>{
      //   console.log('woshi school', data);
      // })
      this.pubid = pubsub.subscribe('hello', function(msgName, data) {
        console.log('有人发布了hello',data);
      })
    },
    beforeDestroy() {
      pubsub.unsubscribe(this.pubid)
    }
    
}
</script>

<style scoped>
  .test {
    background-color: green;
  }
</style>