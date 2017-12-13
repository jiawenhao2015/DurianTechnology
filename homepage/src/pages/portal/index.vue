<template>
  <div class="portal">
    <page-header></page-header>
    <!-- banner -->
    <div class="banner">
      <el-carousel :interval="3000" :height="carouselHeight"  trigger="click">
        <el-carousel-item v-for="banner in banners" :key="banner.bid">
          <img :src="banner.imageUrl" alt="banner">
        </el-carousel-item>
      </el-carousel>
    </div>
    <div class="globalWidth">
      <div class="intro">
        <h2 class="intro-title">定制属于您的互联网服务</h2>
        <p class="intro-content">
          我是介绍文字我是介绍文字我是介绍文字我是介绍文字我是介绍文字我是介绍文字我是介绍文字我是介绍文字我是介绍文字我是介绍文字
        </p>
      </div>
    <!-- figure -->
      <el-row>
        <el-col :xs="8" :sm="8"></el-col>
      </el-row>
    </div>
  </div>
</template>
<script>
  import PageHeader from '../components/Header'
  export default {
    data() {
      return {
        banners: [
          {
            bid: 1,
            imageUrl: 'static/images/banner.png'
          },
          {
            bid: 2,
            imageUrl: 'static/images/banner1.png'
          },
          {
            bid: 3,
            imageUrl: 'static/images/banner2.png'
          },
          {
            bid: 4,
            imageUrl: 'static/images/banner3.png'
          }
        ]
      }
    },
    computed: {
      carouselHeight() {
        if (document.body.offsetWidth < 768) {
          return '200px'
        } else if (document.body.offsetWidth < 992) {
          return '300px'
        } else {
          return '500px'
        }
      }
    },
    components: {
      PageHeader
    },
    methods: {
    }
  }
</script>
<style rel="stylesheet/scss" lang="scss" scoped>
  .portal {
    width: 100%;
    .banner {
      text-align: center;
      margin: 0 auto;
      height: 200px;
      .el-carousel {
        /*width: 100%;*/
        img {
          margin: 0 -100%;
          height: 100%;
        }
      }
    }
    .globalWidth {
      .intro {
        padding: 0 10px;
        width: 100%;
        .intro-title {
          font-size: 24px;
          text-align: center;
          color: #303133;
          padding: 10px;
        }
        .intro-content {
          font-size: 14px;
          line-height: 1.5;
          color: #606266;
        }
      }
    }
  }
  @media screen and (min-width: 768px){
    .portal {
      .banner {
        height: 300px;
      }
      .globalWidth {
        .intro {
          padding: 20px 10px;
          .intro-title {
            font-size: 30px;
          }
          .intro-content {
            font-size: 16px;
          }
        }
      }
    }
  }
  @media screen and (min-width: 992px){
    .portal {
      .banner {
        height: 500px;
      }
    }
  }
</style>
