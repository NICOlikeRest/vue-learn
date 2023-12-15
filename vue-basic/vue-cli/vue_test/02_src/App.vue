<template>
  <div>
    <h1 v-text="msg" ref="title"></h1>
    <button @click="showDOM">点我输出DOM</button>
    <SchoolCom ></SchoolCom>
  </div>
</template>

<script>
import SchoolCom from './components/SchoolCom.vue'
export default {
    name: 'App',
    components:{SchoolCom},
    data() {
        return {
            msg: 'Hello'
        }
    },
    methods: {
        showDOM() {
            // console.log('@@');
            console.log(this.$refs.title);
        }
    },
}
</script>

<style>

</style>