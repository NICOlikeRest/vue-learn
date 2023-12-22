<template>
  
    <div class="container">

      <CategoryCom title="美食">
        <img src="https://avatars.githubusercontent.com/u/79702637?v=4" alt="">
      </CategoryCom>

      <CategoryCom title="游戏">
        <ul>
          <li v-for="(item, index) in games" :key="index">{{ item }}</li>
        </ul>
      </CategoryCom>
      <CategoryCom title="电影">
        <video controls src="http://clips.vorwaerts-gmbh.de/big_buck_bunny.mp4"></video>
      </CategoryCom>
      
    </div>
</template>

<script>
import CategoryCom from './components/CategoryCom.vue'

export default {
  name: "App",
  components:{ CategoryCom },
  data() {
    return {
      foods: ['火锅', '烧烤', '小龙虾', '牛排'],
      games: ['红色警戒', '穿越火线', '劲舞团', '超级玛丽'],
      films: ['《教父》', '《拆弹专家》', '《你好，李焕英》', '《尚硅谷》']
    }
  },

  
}
</script>

<style>
.container {
  display: flex;
  justify-content: space-around;
}
img {
  width: 50%;
  height: 50%;
}
video {
  width: 100%;
}


</style>