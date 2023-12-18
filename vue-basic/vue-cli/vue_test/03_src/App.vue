<template>
  <div>
    
    <StudentCom name='yty' sex='male' :age=18></StudentCom>
    <StudentCom name='yt1y' sex='1male' :age=118></StudentCom>

  </div>
</template>

<script>
import StudentCom from './components/StudentCom.vue'
export default {
    name: 'App',
    components:{StudentCom},
    

}
</script>

<style>

</style>