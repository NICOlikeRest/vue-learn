<template>
  <div class="school">
    <h1 @click="showName">学校名称：{{name}}</h1>  <hr>
    学校地址：{{address}}
  </div>
</template>

<script>
import {mixin} from '../mixin'
export default {
    name: 'SchoolCom',
    data() {
        return {
            name: 'shangguigu',
            address: 'hangzhou'
        }
    },
    mixins:[mixin]
    
}
</script>

<style>
    .school {
        background-color: green;
    }
</style>