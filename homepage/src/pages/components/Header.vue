<template>
  <div class="header">
    <div class="nav_wrapper">
      <div class="nav">
        <div class="logo">
          <h1><a href="#">Durian Technology</a></h1>
        </div>
        <ul class="navbar">
          <li class="nav-item"><a href="#">首页</a></li>
          <li class="nav-item"><a href="#">业务范围</a></li>
          <li class="nav-item"><a href="#">关于我们</a></li>
          <li class="nav-item"><a href="#">联系我们</a></li>
        </ul>
      </div>
    </div>
  </div>
</template>
<script>
  export default {
    data() {
      return {}
    },
    components: {},
    methods: {}
  }
</script>
<style rel="stylesheet/scss" lang="scss" scoped>
  .header {
    width: 100%;
    background: #000;
    height: 60px;
    .nav_wrapper {
      width: 100%;
      .nav {
        width: 100%;
        text-align: center;
        .logo {
          margin: 0 auto;
          color: #fff;
          line-height: 60px;
        }
        .navbar {
          height: 60px;
          float: right;
          .nav-item {
            color: #fff;
            display: inline-block;
            line-height: 60px;
            font-size: 14px;
            padding: 0 20px;
            font-family: "Microsoft YaHei";
            /*width: 100px;*/
            height: 60px;
            a {
              display: inline-block;
              width: 100%;
              text-align: left;
            }
            &:hover {
              color: #878D99;
            }
          }
        }
      }
    }
  }
  @media screen and (min-width: 768px){
    .header {
      .nav_wrapper {
        padding: 0 10px;
        .nav {
          .logo {
            float: left;
          }
        }
      }
    }
  }
  @media screen and (min-width: 1200px){
    .header {
      .nav_wrapper {
        width: 1220px;
        margin: 0 auto;
        .nav {
          .logo {
            float: left;
          }
        }
      }
    }
  }
</style>
