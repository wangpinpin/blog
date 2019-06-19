<template>
  <div class="header">
    <div class="menu-btn">
      <div class="menu"></div>
    </div>
    <h1 class="logo">
      <a href="index.html">
        <span>MYBLOG</span>
        <img src="../../static/img/logo.png">
      </a>
    </h1>
    <div class="nav">
      <a href="index.html" class="active">文章</a>
      <a href="whisper.html">微语</a>
      <a href="leacots.html">留言</a>
      <a href="album.html">相册</a>
      <a href="about.html">关于</a>
    </div>
    <ul class="layui-nav header-down-nav">
      <li class="layui-nav-item"><a href="index.html" class="active">文章</a></li>
      <li class="layui-nav-item"><a href="whisper.html">微语</a></li>
      <li class="layui-nav-item"><a href="leacots.html">留言</a></li>
      <li class="layui-nav-item"><a href="album.html">相册</a></li>
      <li class="layui-nav-item"><a href="about.html">关于</a></li>
    </ul>
    <p class="welcome-text">
      欢迎来到<span class="name">小明</span>的博客~
    </p>
  </div>
</template>

<script>
export default {
  name: 'header',
  props: {
    msg: String,
  },
};
</script>

<style scoped lang="scss">
  .header{
    height: 120px;
    line-height: 120px;
    position: relative;
    font-size: 16px;
  }
  .header .logo,.header .welcome-text,.header .nav{
    position: absolute; top: 0;
  }
  .header .logo{left: 65px;}
  .header .logo span{display: none;}
  .header .nav{left: 250px;}
  .header .nav a{color: #3f2863; margin:0 40px;text-decoration: none;}
  .header .nav a.active{color: #ff7f21;}
  .header .welcome-text{right: 50px;}
  .header .header-down-nav{display: none;}
</style>
