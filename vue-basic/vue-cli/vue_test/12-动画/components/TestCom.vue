<template>
  <div>
    <button @click="isShow = !isShow">显示、隐藏</button>
    <transition name="hello" appear>
    <h1 v-show="isShow">你好啊！</h1>
    </transition>
  </div>
</template>

<script>
export default {
    name: 'TestCom',
    data() {
        return {
            isShow:true
        }
    },
}
</script>

<style>
    h1 {
        background-color: orange;
    }
    .hello-enter-active {
        animation: atguigu 1s;
    }
    .hello-leave-active {
        animation: atguigu 1s reverse;
    }



    @keyframes atguigu {
        from {
            transform: translateX(-100%);
        }
        to {
            transform: translateY(0px);
        }
    }
</style>