<template>
  <div>
    <page-header></page-header>
    <div class="globalWidth contact">
      <el-row>
        <el-col :xs="24"><div class="img"><img src="static/images/connect.jpg" alt=""></div></el-col>
      </el-row>
      <div class="body">
        <div class="inner">
          <el-row :gutter="20">
            <el-col :xs="24" :sm="12" class="item">
              <h2 class="contact-title">联系方式</h2>
              <ul>
                <li>公司：榴莲科技有限公司</li>
                <li>地址：河北省遵化市</li>
                <li>电话：18730236715</li>
                <li>邮箱：contact@durainTech.com</li>
              </ul>
            </el-col>
            <el-col :xs="24" :sm="12" class="item"><div class="img"><img src="static/images/about-left.jpg" alt=""></div></el-col>
          </el-row>
          <el-row :gutter="20">
            <h2 class="con-title">客户服务</h2>
            <el-col :xs="24" :sm="12">
              <ul class="cont">
                <li class="sub-title">客服</li>
                <li class="sub-item">服务热线：18730236715</li>
                <li class="sub-item">Email：DT_KF@durainTech.com</li>
                <li class="sub-item">在线客服：<el-button type="text" size="small">开始咨询</el-button></li>
              </ul>
            </el-col>
            <el-col :xs="24" :sm="12">
              <ul class="cont">
                <li class="sub-title">售后</li>
                <li class="sub-item">联系人：贾文浩</li>
                <li class="sub-item">电话：18701519755</li>
                <li class="sub-item">地址：北京工业大学</li>
              </ul>
            </el-col>
          </el-row>
          <el-row :gutter="20">
            <h2 class="con-title" style="margin-bottom: 30px;">媒体垂询/公关传播</h2>
            <el-col :xs="24">
              <ul class="cont">
                <li class="sub-item">Email: PR@durainTech.com</li>
              </ul>
            </el-col>
          </el-row>
          <el-row :gutter="20">
            <h2 class="con-title">业务合作</h2>
            <el-col :xs="24" :sm="12">
              <ul class="cont">
                <li class="sub-title">市场推广/品牌合作</li>
                <li class="sub-item">Email：marketing@durainTech.com</li>
              </ul>
            </el-col>
            <el-col :xs="24" :sm="12">
              <ul class="cont">
                <li class="sub-title">产品与技术相关战略合作</li>
                <li class="sub-item">Email：cooperation@durainTech.com</li>
              </ul>
            </el-col>
          </el-row>
          <el-row :gutter="20">
            <h2 class="con-title" style="margin-bottom: 30px;">加入榴莲科技</h2>
            <el-col :xs="24">
              <ul class="cont">
                <li class="sub-item">Email: zhaopin@durainTech.com</li>
              </ul>
            </el-col>
          </el-row>
        </div>
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
<style scoped rel="stylesheet/scss" lang="scss">
  .contact{
    overflow: hidden;
    padding-top: 50px;
    font-family:"Microsoft YaHei";
    .img {
      img {
        width: 100%;
      }
    }
    .body {
      padding: 20px;
      margin-top: 20px;
      background: #eee;
      .inner {
        width: 100%;
        overflow: hidden;
        background: #fff;
        padding: 0 30px;
        .el-row {
          border-bottom: 1px dashed #ccc;
          padding-bottom: 40px;
          margin: 50px 0 0;
          .item {
            .contact-title {
              font-weight:lighter;
              font-size: 24px;
              padding: 30px 0;
            }
            ul {
              li {
                padding-top: 25px;
              }
            }
            .img {
              img {
                width: 100%;
              }
            }
          }
          .con-title {
            font-size: 19px;
            font-weight: lighter;
            padding-left: 15px;
          }
          .el-col {
            .cont {
              .sub-title {
                font-size: 16px;
                color: #303133;
                font-weight: bold;
                padding: 20px 5px 10px;
              }
              .sub-item {
                color: #909399;
                padding: 5px;
              }
            }
          }
        }
      }
    }
  }
</style>

