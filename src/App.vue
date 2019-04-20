<template>
  <div id="app">
    <!--除了exclude，还可以使用activated，参考Home.vue-->
    <!--Bug: exclude导致Detail页面Header滚动渐变效果消失，可以使用上面讲的Home页面处理方式规避-->
    <keep-alive exclude="Detail">
      <router-view/>
    </keep-alive>
  </div>
</template>

<script>
  export default {
    name: 'App'
  }
</script>

<style>
</style>
