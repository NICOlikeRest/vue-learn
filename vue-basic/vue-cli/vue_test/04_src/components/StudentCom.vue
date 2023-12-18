<template>
  <div>
    <div v-text='msg'></div> <hr>
    <h2 @click="showName">学生名称：{{name}}</h2>  <hr>
    学生性别：{{sex}} <hr>

  </div>
</template>

<script>
import {mixin} from '../mixin'
export default {
    name: 'SchoolCom',
    data() {
        return {
            msg: 'hello',
            name:'yty',
            sex:'male'
        }
    },
    mixins:[mixin]

    // props:['name', 'age', 'sex']
    // props: {
    //   name:String,
    //   age:Number,
    //   sex:String
    // }
}
</script>

<style>

</style>