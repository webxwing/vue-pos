<template>
  <div id="app">
    <!--左侧导航-->
    <leftMenu></leftMenu>
    <div class="main">
      <router-view></router-view>
    </div>
  </div>
</template>

<script>
  import leftMenu from '@/components/Common/LeftMenu'
  export default {
    name: 'app',
    components:{
      leftMenu
    }
  }
</script>

<style>
  #app {
    font-family: 'Microsoft YaHei UI Light','Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    height:100%;
  }
  .main{
    float:left;
    width:95%;
    background-color:#EFF2F7;
    height:100%;
    overflow:auto;
  }
</style>
