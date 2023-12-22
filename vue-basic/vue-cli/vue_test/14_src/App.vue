<template>
  
    <div class="container">
      <SearchCom/>
      <ListCom/>
    </div>
</template>

<script>
import SearchCom from './components/SearchCom.vue'
import ListCom from './components/ListCom.vue'
export default {
  name: "App",
  components:{ SearchCom , ListCom }

  
}
</script>

<style>



</style>