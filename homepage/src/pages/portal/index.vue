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
      <el-row class="figure" :gutter="figureGutter">
        <el-col :xs="8" :sm="8"><div class="img"><div class="word">网站制作</div><img src="static/images/figure1.png" alt=""></div></el-col>
        <el-col :xs="8" :sm="8"><div class="img"><div class="word">小程序</div><img src="static/images/figure2.png" alt=""></div></el-col>
        <el-col :xs="8" :sm="8"><div class="img"><div class="word">运营推广</div><img src="static/images/figure3.png" alt=""></div></el-col>
      </el-row>
    </div>
    <div class="wrapper gray">
      <div class="globalWidth">
        <el-row>
          <el-col :span="24" class="rowHeight">
            <div class="title">
              <h2>服务内容</h2>
              <i class="el-icon-more"></i>
            </div>
          </el-col>
        </el-row>
        <el-row :gutter="10">
          <el-col :xs="12" :sm="6" v-for="item in service" :key="item.sid">
            <div class="service">
              <svg-icon :icon-class="item.icon"></svg-icon>
              <h3 class="ser-title">{{ item.title }}</h3>
              <h4 class="ser-subTitle">
                {{ item.subtitle }}
              </h4>
              <ul class="ser-cont">
                <li v-for="(cont, index) in item.content" :key="index">{{ cont }}</li>
              </ul>
            </div>
          </el-col>
        </el-row>
      </div>
    </div>
    <div class="wrapper white">
      <div class="globalWidth">
        <el-row>
          <el-col :span="24" class="rowHeight">
            <div class="title">
              <h2>成功案例</h2>
              <i class="el-icon-more"></i>
            </div>
          </el-col>
        </el-row>
        <el-row :gutter="10">
          <el-col :xs="12" :sm="6" v-for="item in service" :key="item.sid">
            <div class="service">
              <svg-icon :icon-class="item.icon"></svg-icon>
              <h3 class="ser-title">{{ item.title }}</h3>
              <h4 class="ser-subTitle">
                {{ item.subtitle }}
              </h4>
              <ul class="ser-cont">
                <li v-for="(cont, index) in item.content" :key="index">{{ cont }}</li>
              </ul>
            </div>
          </el-col>
        </el-row>
      </div>
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
        ],
        service: [
          {
            sid: 1,
            icon: 'computer',
            title: '高端网站',
            subtitle: '高端行业、品牌网站 一站式解决方案',
            content: [
              '企业集团官网',
              '品牌营销网站',
              '行业信息平台',
              '响应式网站升级'
            ]
          },
          {
            sid: 2,
            icon: 'iPhone',
            title: '移动应用',
            subtitle: '移动互联网产品定制 运营服务',
            content: [
              'iOS app',
              'Android app',
              'H5移动微应用',
              'PWA渐进式web应用',
            ]
          },
          {
            sid: 3,
            icon: 'wechat',
            title: '微信服务',
            subtitle: '全方位定制属于您的微信服务',
            content: [
              '定制小程序',
              '公众号主页',
              '公众号文章',
              '微信服务号定制'
            ]
          },
          {
            sid: 4,
            icon: 'product',
            title: '产品规划',
            subtitle: '符合企业定位、业务可落地验证的规划服务',
            content: [
              '产品策略规划',
              '用户体验研究',
              'UI创意设计',
              '产品设计制作'
            ]
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
      },
      figureGutter() {
        if (document.body.offsetWidth < 768) {
          return 10
        } else if (document.body.offsetWidth < 992) {
          return 20
        } else {
          return 30
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
      padding: 0 10px;
      margin-bottom: 10px;
      .intro {
        width: 100%;
        .intro-title {
          font-size: 24px;
          text-align: center;
          color: #303133;
          padding: 10px 0;
        }
        .intro-content {
          font-size: 14px;
          line-height: 1.5;
          color: #606266;
        }
      }
      .figure {
        .img {
          position: relative;
          cursor: pointer;
          img {
            width: 100%;
          }
          .word {
            color: #fff;
            width: 100%;
            font-size: 14px;
            font-family: "Microsoft YaHei";
            position: absolute;
            text-align: center;
            left: 0;
            top: 50%;
            transform: translateY(-50%);
          }
        }
      }
    }
    .gray {
      background: #F8F8F8;
      .title {
        .el-icon-more {
          background: #F8F8F8;
        }
      }
    }
    .white {
      background: #fff;
      .title {
        .el-icon-more {
          background: #fff;
        }
      }
    }
    .wrapper {
      .globalWidth {
        .title {
          font-size: 16px;
          font-family: "Microsoft YaHei";
          border-bottom: 1px solid #6a6a6a;
          width: 200px;
          margin: 15px auto;
          position: relative;
          h2 {
            font-weight: lighter;
            letter-spacing: 5px;
            color: #6a6a6a;
            margin: 15px 0;
            text-align: center;
          }
          .el-icon-more {
            position: absolute;
            width: 50px;
            font-size: 20px;
            left: 50%;
            margin-left: -25px;
            bottom: -10px;
            color: #2489e9;
            text-align: center;
          }
        }
        .service {
          text-align: center;
          margin-bottom: 10px;
          .svg-icon {
            font-size: 70px;
            color: #666666;
          }
          .ser-title {
            margin: 10px 0;
            font-size: 22px;
            font-weight: lighter;
          }
          .ser-subTitle {
            margin-bottom: 10px;
            color: #606266;
          }
          .ser-cont {
            line-height: 1.5;
            color: #909399;
          }
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
        padding: 0 20px;
        margin-bottom: 20px;
        .intro {
          padding: 20px 10px;
          .intro-title {
            font-size: 30px;
          }
          .intro-content {
            font-size: 16px;
          }
        }
        .figure {
          .img {
            .word {
              font-size: 22px;
            }
          }
        }
      }
      .wrapper {
        .globalWidth {
          .title {
            font-size: 20px;
            h2 {
              font-size: 30px;
              margin: 25px 0;
            }
            .el-icon-more {
              width: 50px;
              font-size: 30px;
              bottom: -15px;
            }
          }
          .service {
            text-align: center;
            .svg-icon {
              font-size: 100px;
            }
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
