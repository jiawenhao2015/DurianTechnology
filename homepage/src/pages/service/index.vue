<template>
  <div>
    <page-header></page-header>
    <div class="globalWidth" :style="{minHeight: minHeight}">
      <div class="wrapper">
        <h2 class="top-title">
          业务服务
        </h2>
        <el-row :gutter="20" class="service">
          <el-col :xs="24" :sm="8" v-for="item in serviceList" :key="item.id">
            <h3 class="ser-title">{{ item.title }}</h3>
            <p class="content">
              {{ item.content }}
            </p>
            <div class="ser-img">
              <img :src="item.imageUrl" alt="">
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
      return {
        serviceList: [
          {
            id: 1,
            title: '行业定制服务',
            content: '提供基于企业所在行业的行业整体解决方案服务。从企业的定位出发，围绕企业所在行业的行业痛点分析，业务模式梳理，提供行业定制服务。',
            imageUrl: 'static/images/service-1.png'
          },
          {
            id: 2,
            title: '战略定制服务',
            content: '提供基于企业战略的定制服务。从企业的互联网战略目标出发，围绕企业互联网营销战略、技术开发战略、人才战略，提供战略定制服务。',
            imageUrl: 'static/images/service-2.png'
          },
          {
            id: 3,
            title: '产品定制服务',
            content: '提供企业互联网产品的策划、体验、运营的定制服务。从企业的市场战略、业务需求出发，进行市场调研、需求分析、用户体验分析，提供产品定制服务。',
            imageUrl: 'static/images/service-3.png'
          }
        ]
      }
    },
    computed: {
      minHeight() {
        return document.documentElement.clientHeight - 123 + 'px'
      }
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
    .service {
      .ser-title {
        color: #606266;
        text-align: center;
        font-size: 20px;
        margin-bottom: 20px;
      }
      .content {
        color: #909399;
        line-height: 1.5;
        text-align: justify;
        margin: 0 10px 20px;
        height: 100px;
      }
      .ser-img {
        text-align: center;
        padding: 0 10px;
        img {
          width: 100%;
        }
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
      .service {
        .content {
          margin: 0 10px 40px;
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
