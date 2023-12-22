<template>
  
    <div class="container">


      <CategoryCom title="游戏">
        <ul >
          <li v-for="(item, index) in games" :key="index">{{ item }}</li>
        </ul>
      </CategoryCom>


      <CategoryCom title="游戏">
          <ul >
            <li v-for="(item, index) in games" :key="index">{{ item }}</li>
          </ul>
        </CategoryCom>





        <CategoryCom title="游戏">
          <ul >
            <li v-for="(item, index) in games" :key="index">{{ item }}</li>
          </ul>
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
      games: ['红色警戒', '穿越火线', '劲舞团', '超级玛丽'],
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