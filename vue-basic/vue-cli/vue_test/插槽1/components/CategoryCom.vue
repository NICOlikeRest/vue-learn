<template>
  <div class="categroy">
    <h3>{{title}}分类</h3>
    <!-- <ul>
        <li v-for="(item, index) in listData" :key="index">{{ item }}</li>
    </ul> -->
    <slot>我是默认值</slot>
  </div>
</template>

<script>
    export default {
        name:"CategoryCom",
        props:[ 'title']
    }
</script>

<style>
.categroy {
    background-color: skyblue;
    width: 200px;
    height: 200px;
}
h3 {
    text-align: center;
    background-color: orange;
}
</style>