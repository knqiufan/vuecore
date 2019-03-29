<template>
    <div class="fly-header layui-bg-black">
    <div class="layui-container">
      <a class="fly-logo" href="/">
        <img src="../assets/logo01.png" alt="layui">
      </a>
      <ul class="layui-nav fly-nav layui-hide-xs">
        <li class="layui-nav-item layui-this">
          <a href="/"><i class="iconfont icon-jiaoliu"></i>交流</a>
        </li>
        <li class="layui-nav-item">
          <a href=""><i class="iconfont icon-iconmingxinganli"></i>案例</a>
        </li>
        <li class="layui-nav-item">
          <a href="#" target="_blank"><i class="iconfont icon-ui"></i>框架</a>
        </li>
      </ul>
      
      <ul class="layui-nav fly-nav-user">
        
        <!-- 未登入的状态 -->
        <!-- <li class="layui-nav-item">
          <a class="iconfont icon-touxiang layui-hide-xs" href=""></a>
        </li>
        <li class="layui-nav-item">
          <a href="">登入</a>
        </li>
        <li class="layui-nav-item">
          <a href="">注册</a>
        </li>
        <li class="layui-nav-item layui-hide-xs">
          <a href="" onclick="layer.msg('正在通过QQ登入', {icon:16, shade: 0.1, time:0})" title="QQ登入" class="iconfont icon-qq"></a>
        </li>
        <li class="layui-nav-item layui-hide-xs">
          <a href="" onclick="layer.msg('正在通过微博登入', {icon:16, shade: 0.1, time:0})" title="微博登入" class="iconfont icon-weibo"></a>
        </li> -->
      </ul>
    </div>
  </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
.fly-header{background-color:#404553!important;position: fixed; left: 0; top: 0; z-index: 10000; width: 100%; height: 60px; border-bottom: 1px solid #404553; border-right: 1px solid #404553; border-radius: 0;}
.fly-header .layui-nav{padding: 0; background: none;}
.fly-header .fly-nav a{padding: 0 25px 0 60px;}
.fly-header .fly-nav-user li a{padding: 0 10px;}
.fly-header .fly-nav-user li .fly-nav-avatar{padding-right: 0;}
.fly-header .fly-nav-user a.iconfont{color: #A9B7B7;}
.fly-header>.layui-nav-item a{color: rgba(255,255,255,0.5);}
.fly-header .layui-this a{color: #fff;}
.fly-header .layui-nav .layui-this:after,
.fly-header .layui-nav .layui-nav-bar,
.fly-header .fly-nav-user .layui-nav-more{display: none !important;}
.fly-header .fly-nav-user .layui-nav-child{left: auto; right: 0; width: 120px; min-width: 0;}
.fly-header .fly-nav-user li .fly-nav-avatar{padding-right: 15px;}
.fly-header .fly-nav-user{margin-right: 5px;}
.layui-container{position:relative;margin:0 auto;padding:0 15px;box-sizing:border-box}
.fly-logo{position: absolute; left: 15px }
@media screen and (min-width:768px){.layui-container{width:750px}}
@media screen and (min-width:992px){.layui-container{width:970px}}
@media screen and (min-width:1200px){.layui-container{width:1170px}}
.layui-nav{position:relative;padding:0 20px;background-color:#393D49;color:#fff;border-radius:2px;font-size:0;box-sizing:border-box}
.layui-nav *{font-size:14px}
.layui-nav .layui-nav-item{position:relative;display:inline-block;*display:inline;*zoom:1;vertical-align:middle;line-height:60px}
.layui-nav .layui-nav-item a{display:block;padding:0 20px;color:#fff;color:rgba(255,255,255,.7);transition:all .3s;-webkit-transition:all .3s}
.layui-nav .layui-this:after,.layui-nav-bar,.layui-nav-tree .layui-nav-itemed:after{position:absolute;left:0;top:0;width:0;height:5px;background-color:#5FB878;transition:all .2s;-webkit-transition:all .2s}
.layui-nav-bar{z-index:1000}
.layui-nav .layui-nav-item a:hover,.layui-nav .layui-this a{color:#fff}
.layui-nav .layui-this:after{content:'';top:auto;bottom:0;width:100%}
.layui-nav-img{width:30px;height:30px;margin-right:10px;border-radius:50%}
.layui-nav .layui-nav-more{content:'';width:0;height:0;border-style:solid dashed dashed;border-color:#fff transparent transparent;overflow:hidden;cursor:pointer;transition:all .2s;-webkit-transition:all .2s;position:absolute;top:50%;right:3px;margin-top:-3px;border-width:6px;border-top-color:rgba(255,255,255,.7)}
.layui-nav .layui-nav-mored,.layui-nav-itemed .layui-nav-more{margin-top:-9px;border-style:dashed dashed solid;border-color:transparent transparent #fff}
.layui-nav-child{display:none;position:absolute;left:0;top:65px;min-width:100%;line-height:36px;padding:5px 0;box-shadow:0 2px 4px rgba(0,0,0,.12);border:1px solid #d2d2d2;background-color:#fff;z-index:100;border-radius:2px;white-space:nowrap}
.layui-nav .layui-nav-child a{color:#333}
.layui-nav .layui-nav-child a:hover{background-color:#f2f2f2;color:#000}
.layui-nav-child dd{position:relative}
.layui-nav .layui-nav-child dd.layui-this a,.layui-nav-child dd.layui-this{background-color:#5FB878;color:#fff}
.layui-nav-child dd.layui-this:after{display:none}
.layui-nav-tree{width:200px;padding:0}
.layui-nav-tree .layui-nav-item{display:block;width:100%;line-height:45px}
.layui-nav-tree .layui-nav-item a{height:45px;line-height:45px;text-overflow:ellipsis;overflow:hidden;white-space:nowrap}
.layui-nav-tree .layui-nav-item a:hover{background-color:#4E5465}
.layui-nav-tree .layui-nav-bar{width:5px;height:0;background-color:#009688}
.layui-nav-tree .layui-nav-child dd.layui-this,.layui-nav-tree .layui-nav-child dd.layui-this a,.layui-nav-tree .layui-this,.layui-nav-tree .layui-this>a,.layui-nav-tree .layui-this>a:hover{background-color:#009688;color:#fff}
.layui-nav-tree .layui-this:after{display:none}
.layui-nav-itemed>a,.layui-nav-tree .layui-nav-title a,.layui-nav-tree .layui-nav-title a:hover{color:#fff!important}
.layui-nav-tree .layui-nav-child{position:relative;z-index:0;top:0;border:none;box-shadow:none}
.layui-nav-tree .layui-nav-child a{height:40px;line-height:40px;color:#fff;color:rgba(255,255,255,.7)}
.layui-nav-tree .layui-nav-child,.layui-nav-tree .layui-nav-child a:hover{background:0 0;color:#fff}
.layui-nav-tree .layui-nav-more{top:20px;right:10px;margin:0}
.layui-nav-itemed .layui-nav-more{top:14px}
.layui-nav-itemed .layui-nav-child{display:block;padding:0;background-color:rgba(0,0,0,.3)!important}
.layui-nav-side{position:fixed;top:0;bottom:0;left:0;overflow-x:hidden;z-index:999}
.layui-bg-blue .layui-nav-bar,.layui-bg-blue .layui-nav-itemed:after,.layui-bg-blue .layui-this:after{background-color:#93D1FF}
.layui-bg-blue .layui-nav-child dd.layui-this{background-color:#1E9FFF}
.layui-bg-blue .layui-nav-itemed>a,.layui-nav-tree.layui-bg-blue .layui-nav-title a,.layui-nav-tree.layui-bg-blue .layui-nav-title a:hover{background-color:#007DDB!important}
</style>



