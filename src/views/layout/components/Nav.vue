<template>
    <div class="fly-header layui-bg-black">
    <div class="layui-container">
      <a class="fly-logo" href="/">
        <img src="../assets/logo01.png" alt="layui">
      </a>
      <el-menu
        :default-active="activeIndex2"
        class="el-menu"
        mode="horizontal"
        @select="handleSelect"
        background-color="#545c64"
        text-color="#fff"
        active-text-color="#ffd04b">
        <el-menu-item index="1"><i class="el-icon-service"></i>交流</el-menu-item>
        <el-menu-item index="3"><i class="el-icon-message"></i>消息中心</el-menu-item>
        <el-menu-item index="4"><i class="el-icon-printer"></i>我的工作台</el-menu-item>
        <el-submenu index="2">
          <template slot="title"><i class="el-icon-menu"></i>其他</template>
          <el-menu-item index="2-1">选项1</el-menu-item>
          <el-menu-item index="2-2">选项2</el-menu-item>
          <el-menu-item index="2-3">选项3</el-menu-item>
          <el-submenu index="2-4">
            <template slot="title">选项4</template>
            <el-menu-item index="2-4-1">选项1</el-menu-item>
            <el-menu-item index="2-4-2">选项2</el-menu-item>
            <el-menu-item index="2-4-3">选项3</el-menu-item>
          </el-submenu>
        </el-submenu>
        <el-button class="login" type="info">
          登录
        </el-button>
        <el-button class="region" type="info">
          注册
        </el-button>
      </el-menu>
    </div>
  </div>
  
</template>

<script>
export default {
    data() {
      return {
        activeIndex: '1',
        activeIndex2: '1'
      };
    },
    methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath)
      }
    }
}
</script>

<style scoped>
.fly-header{background-color:rgb(84, 92, 100)!important;position: fixed; left: 0; top: 0; z-index: 10000; width: 100%; height: 60px; border-bottom: 1px solid rgb(84, 92, 100); border-right: 1px solid rgb(84, 92, 100); border-radius: 0;}
.fly-header .layui-nav{padding: 0; background: none;float: right;}
.fly-header .layui-nav .layui-nav-item{display: inline-block;line-height: 60px;position: relative;vertical-align:middle;}
.fly-header .fly-nav a{padding: 0 25px 0 60px;}
.fly-header .fly-nav-user li a{padding: 0 10px;}
.fly-header .fly-nav-user li .fly-nav-avatar{padding-right: 0;}
.fly-header .fly-nav-user a.iconfont{color: #A9B7B7;}
.fly-header>.layui-nav-item a{display:block;padding:0 20px;color:#fff;color:rgba(255,255,255,.7);transition:all .3s;-webkit-transition:all .3s}
.fly-header .layui-this a{color: #fff;}
.fly-header .layui-nav .layui-this:after,
.fly-header .layui-nav .layui-nav-bar,
.fly-header .fly-nav-user .layui-nav-more{display: none !important;}
.fly-header .fly-nav-user .layui-nav-child{left: auto; right: 0; width: 120px; min-width: 0;}
.fly-header .fly-nav-user li .fly-nav-avatar{padding-right: 15px;}
.fly-header .fly-nav-user{margin-right: 5px;}
.layui-container{position:relative;margin:0 auto;padding:0 15px;box-sizing:border-box}
.el-menu{position:relative;margin-left:25%}
/* .el-menu .login{color:#fff;display: inline-block;line-height: 60px;font-size: 15px} */
.fly-logo{position: absolute; left: 15px;top:10px}
.layui-container .el-menu .login,.layui-container .el-menu .region{margin-top:10px;}
@media screen and (min-width:768px){.el-menu,.layui-container{width:750px}}
@media screen and (min-width:992px){.el-menu,.layui-container{width:970px}}
@media screen and (min-width:1200px){.el-menu,.layui-container{width:1170px}}
</style>



