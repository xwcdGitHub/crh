<template>
  <div id="app">
    <!--header-->
    <c-header></c-header>
    <!--header-->
    <main>
      <!-- 左侧导航 -->
      <c-nav></c-nav>
      <!-- 右侧主内容区 -->
      <user></user>
    </main>
  </div>
</template>

<script>
  import CHeader from './components/c-header/c-header.vue'
  import CNav from './components/c-nav/c-nav.vue'
  import CTable from './components/c-table/c-table.vue'
  import User from './components/user/user.vue'

  export default {
    components: {
      CHeader,
      CNav,
      CTable,
      User
    }
  }
</script>

<style>
  body{
    margin: 0;
  }
  #app {
    font-family: Helvetica, sans-serif;
    text-align: center;
    overflow: hidden;
  }
  main{
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    min-height: 800px;
    background-color: #FCFCFC;
  }


</style>
