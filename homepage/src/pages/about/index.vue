<template>
  <div>
    <page-header></page-header>
    <div class="globalWidth">
      <div class="wrapper">
        <h2 class="top-title">
          关于榴莲科技
        </h2>
        <el-row :gutter="20">
          <el-col :xs="24" :sm="24">
            <div class="img">
              <img src="static/images/about-banner.jpg" alt="">
            </div>
          </el-col>
          <el-col :xs="24" :sm="12"><div class="img"><img src="static/images/about-left.jpg" alt=""></div></el-col>
          <el-col :xs="24" :sm="12">
            <div class="word">
              <div class="intro">
                榴莲科技有限公司是2017年12月9日由一群小伙子一时兴起创建的一家以互联网商业模式创新及软件产品技术创新为核心，标准化管理、快速发展的国家级高新技术企业。公司位于河北省遵化市，其地理位置优越，交通便利。公司致力于为中小型企业提供私人定制的互联网服务以及后续的一系列增值服务，让每一个企业都能享受到互联网的便利。
              </div>
              <div class="intro">
                在 “互联网+”战略成为企业经济增长新引擎的形势下，榴莲科技专注研究企业在“互联网+”进程中的痛点与需求，依托公司10多年互联网产品技术及方法论沉淀为企业提供商业模式咨询策划、互联网产品研发、供应链金融及保险定制四位一体的解决方案，帮助企业降低试错成本，加速互联网化转型。
              </div>
            </div>
          </el-col>
        </el-row>
      </div>
    </div>
    <page-footer></page-footer>
  </div>
</template>
<script>
  import PageHeader from '../components/Header'
  import PageFooter from '../components/Footer'
  export default {
    data() {
      return {}
    },
    components: {
      PageHeader,
      PageFooter
    },
    methods: {}
  }
</script>
<style rel="stylesheet/scss" lang="scss" scoped>
  .wrapper {
    .top-title {
      padding: 70px 0 20px;
      text-align: center;
      font-family: "Microsoft YaHei";
      font-size: 24px;
      font-weight: lighter;
      border-bottom: 1px solid #DCDFE6;
      margin-bottom: 20px;
    }
    .img {
      margin-bottom: 20px;
      img {
        width: 100%;
      }
    }
    .word {
      .intro {
        font-family: "Microsoft YaHei";
        font-size: 16px;
        color: #475669;
        line-height: 1.5;
        text-indent: 2em;
        padding: 0 10px;
        margin-bottom: 40px;
        margin-top: 10px;
      }
    }
  }
  @media screen and (min-width: 768px) {
    .wrapper {
      .top-title {
        text-align: left;
        padding: 70px 0 20px 50px;
        margin-bottom: 40px;
      }
      .word {
        .intro {
          margin-top: 50px;
        }
      }
    }
  }
  @media screen and (min-width: 1200px) {
    .wrapper {
      .top-title {
        padding: 70px 0 20px;
      }
    }
  }
</style>
