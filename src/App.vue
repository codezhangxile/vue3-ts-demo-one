<template>
  <div class="head-bar">
    <router-link active-class="router-link-active" to="/">home</router-link>
    <router-link active-class="router-link-active" to="/router">router</router-link>
  </div>


  <router-view />
</template>

<script lang="ts">
import { defineComponent } from 'vue'


export default defineComponent({
  name: 'App',
  components: {
  }
})
</script>

<style lang="scss" >
#app{
  .head-bar{
    height: 40px;
    a{
      display: inline-block;
      text-decoration: none;
      width: 80px;
      height: 40px;
      line-height: 40px;
      text-align: center;
      border: 1px solid blue;
      background-color: black;
      color: #fff;
    }
    .router-link-active{
      color: red;
    }
  }


}
</style>
