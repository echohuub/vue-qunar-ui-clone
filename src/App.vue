<template>
  <div id="app">
    <!--除了exclude，还可以使用activated，参考Home.vue-->
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
