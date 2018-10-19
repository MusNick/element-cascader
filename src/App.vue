
<template>
  <div id="app">
    <h1>前端地址级联</h1>
    <el-cascader
      placeholder="试试搜索：指南"
      v-model="selectAddress"
      :options="options"
      filterable
    ></el-cascader>
  </div>
</template>


<script>
import HelloWorld from './components/HelloWorld.vue'
import address from '../static/area/address.json'

export default {
  name: 'app',
  components: {
    HelloWorld
  },
  data () {
    return {
      options: address,
      selectAddress: []
    }
  },
  methods: {
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>