<template>
  <div id="wrapper">
    <nav class="navbar navbar-inverse">
      <div class="container">
        <a class="navbar-brand" href="#"><i class="glyphicon glyphicon-time">计划表</i></a>
        <ul class="nav navbar-nav">
          <li><router-link to="'/home'">首页</router-link></li>
          <li><router-link to="/time-entries">计划列表</router-link></li>
        </ul>
      </div>
    </nav>
    <div class="container">
      <div class="col-sm-3">
        <sider-bar></sider-bar>
      </div>
      <div class="col-sm-9">
        <router-view></router-view>
      </div>
    </div>
  </div>
</template>
<script>
  import Siderbar from './components/Siderbar.vue';
  export default{
    components:{
      'sider-bar':Siderbar
    }
  }
</script>
<style>
    #wrapper{
        background:url(http://p1.gexing.com/shaitu/20121110/1200/509dd142eefea.jpg) no repeat;
        background-size:cover;
    }
</style>