<template>
  <div id="app">
    <div id="app-1">
        <img src="./assets/logo.png">
        <div>
        <el-button @click="startHacking">Start</el-button>
        </div>
    </div>
    <route-view>
  </div>
</template>

<script>
export default {
  methods: {
    startHacking () {
      this.$notify({
        title: 'It works!',
        type: 'success',
        message: 'We\'ve laid the ground work for you. It\'s time for you to build something epic!',
        duration: 5000
      })
    }
  }
}
</script>

<style>
#app-1 {
  font-family: Helvetica, sans-serif;
  text-align: center;
}
* {
    box-sizing: border-box;
    padding: 0;
    margin: 0;
}
ol,
ul {
    list-style: none;
}
a {
    text-decoration: none;
}

html,
body {
    margin: 0;
    padding: 0;
    height: 100%;
    font-size: 14px;
    background-color: aquamarine;
    font-family: 'Source Sans Pro', 'Helvetica Neue', Helvetica, Arial,
        sans-serif, 'Microsoft YaHei', '微软雅黑', STXihei, '华文细黑', serif;
}

::-webkit-scrollbar {
    width: 4px;
    height: 8px;
}

::-webkit-scrollbar-track {
    background-color: rgba(255, 255, 255, 1);
}

::-webkit-scrollbar-thumb {
    background-color: rgba(135, 141, 153, 0.5);
}
</style>
