<template>
  <div>
    <page-header></page-header>
    <!--<div class="contact">-->
      <!--<div class="contact-cont">-->
        <!--<div class="head">-->
          <!--<img src="static/images/contact.jpg" alt="">-->
        <!--</div>-->
        <!--<div class="body">-->
          <!--<div class="inner">-->
            <!--<div class="left">-->
              <!--<h1>联系方式</h1>-->
              <!--<p>公司：北京哈维思特饲料制造有限公司</p>-->
              <!--<p>&emsp;&emsp;&emsp;Beijing Haweisite Feed manufacturing Co.,Ltd</p>-->
              <!--<p>地址：北京市顺义区牛栏山镇牛富路12号</p>-->
              <!--<p>电话：010-69417256</p>-->
              <!--<p>邮箱：haweisite@163.com</p>-->
            <!--</div>-->
            <!--<div class="right">-->
              <!--<img src="static/images/address.png" alt="">-->
            <!--</div>-->
            <!--<div class="word">-->
              <!--<div class="word-item">-->
                <!--<h3>客户服务</h3>-->
                <!--<div class="word-cont">-->
                  <!--<div class="word-cont-left">-->
                    <!--<h4>客服</h4>-->
                    <!--<p>服务热线：010-69417256</p>-->
                    <!--<p>Email：HW_KF@haweisite.com</p>-->
                    <!--<p>在线客服：开始咨询</p>-->
                  <!--</div>-->
                  <!--<div class="word-cont-right">-->
                    <!--<h4>售后</h4>-->
                    <!--<p>联系人：哈维思特&emsp;&emsp;&emsp;电话：010-69417256</p>-->
                    <!--<p>地址：北京市顺义区牛栏山镇牛富路12号</p>-->
                    <!--<p>邮编：101301</p>-->
                  <!--</div>-->
                <!--</div>-->
              <!--</div>-->
              <!--<div class="word-item">-->
                <!--<h3>媒体垂询/公关传播</h3>-->
                <!--<div class="word-cont">-->
                  <!--<div class="word-cont-left">-->
                    <!--<p>Email：PR@haweisite.com</p>-->
                  <!--</div>-->
                <!--</div>-->
              <!--</div>-->
              <!--<div class="word-item">-->
                <!--<h3>业务合作</h3>-->
                <!--<div class="word-cont">-->
                  <!--<div class="word-cont-left">-->
                    <!--<h4>市场推广/品牌合作</h4>-->
                    <!--<p>Email：marketing@haweisite.com</p>-->
                    <!--<h4>认证店加盟</h4>-->
                    <!--<p>电话：010-69417256</p>-->
                    <!--<p>Email：join@haweisite.com</p>-->
                    <!--<p>(周一至周日9:00-12:00，13:30-18:00，法定节假日除外）</p>-->
                  <!--</div>-->
                  <!--<div class="word-cont-right">-->
                    <!--<h4>经销商服务</h4>-->
                    <!--<p>Email：business@haweisite.com</p>-->
                    <!--<h4>B2C电子商务渠道</h4>-->
                    <!--<p>Email：e-business@haweisite.com</p>-->
                    <!--<h4>产品与技术相关战略合作</h4>-->
                    <!--<p>Email：cooperation@haweisite.com</p>-->
                  <!--</div>-->
                <!--</div>-->
              <!--</div>-->
              <!--<div class="word-item">-->
                <!--<h3>加入哈维思特</h3>-->
                <!--<div class="word-cont">-->
                  <!--<div class="word-cont-left">-->
                    <!--<p>Email：zhaopin@haweisite.com</p>-->
                  <!--</div>-->
                <!--</div>-->
              <!--</div>-->
              <!--<div class="word-item">-->
                <!--<h3>反商业贿赂</h3>-->
                <!--<div class="word-cont">-->
                  <!--<p>哈维思特严禁员工向业务合作伙伴索贿或收取佣金、回扣或其他私人利益。对有具体线索的举报，哈维思特内控合规部门将开展独立调查并为举报人保密。</p>-->
                  <!--<p>Email: lianzheng@haweisite.com</p>-->
                <!--</div>-->
              <!--</div>-->
            <!--</div>-->
          <!--</div>-->
        <!--</div>-->
      <!--</div>-->
      <!---->
    <!--</div>-->
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
  .contact-cont{
    margin: 0 auto;
    width: 1200px;

  }
  .contact-cont .body{
    width: 100%;
    padding: 20px;
    margin-top: 20px;
    box-sizing: border-box;
    background: #eee;
  }
  .contact-cont .body .inner{
    width: 100%;
    overflow: hidden;
    background: #fff;
  }
  .inner .left{
    width: 500px;
    height: 410px;
    padding: 30px;
    box-sizing: border-box;
    float: left;
    margin-right: 30px;
    font-family:"Microsoft YaHei";
  }
  .inner .left h1{
    font-weight:lighter;
    font-size: 24px;
    padding: 30px 0;
  }
  .inner .left p{
    padding-top: 25px;
  }
  .inner .right{
    margin-top: 10px;
  }
  .inner .word{
    margin-top: 30px;
    width: 100%;
  }
  .word .word-item{
    border-top: 1px dashed #ccc;
    /*border-bottom: 1px dashed #ccc;*/
    width: 100%;
    padding: 30px 0;
  }
  .word .word-item h3{
    padding: 20px;
    font-weight:lighter;
  }
  .word .word-item .word-cont{
    width: 100%;
    /*background: red;*/
    overflow: hidden;
  }
  .word-cont .word-cont-left{
    float: left;
    margin-left: 20px;
  }
  .word-cont .word-cont-right{
    float: right;
    width: 50%;
  }
  .word-cont-left h4,.word-cont-right h4{
    padding: 10px 5px;
  }
  .word-cont-left p,.word-cont-right p{
    font-weight:lighter;
    font-size: 15px;
    color:#777;
    padding: 5px;
  }
  .word-cont>p{
    font-weight:lighter;
    font-size: 15px;
    color:#777;
    padding: 5px;
    margin-left: 20px;
  }
</style>

