<template>
  <el-menu :default-active="activeIndex2" class="footer-el-menu-footer" mode="horizontal">
    <div class="footer-centent">
      <div class="footer-centent-text">
        Copyright &copy; 2005-2017 冀ICP备16017666号-1 榴莲科技旗下产品 榴莲云平台提供计算支持
      </div>
    </div>
  </el-menu>
</template>

<script>

  export default {
    data() {
      return {
        activeIndex2: '1'
      }
    },
    methods: {
    }
  }
</script>
<style rel="stylesheet/scss" lang="scss" scoped>
  .footer {
    position: absolute;
    bottom: 0;
    width: 100%;
  }

  .footer-el-menu-footer {
    /*position: absolute;*/
    bottom: 0;
    width: 100%;
    height: 63px;
    background-color: #202a39;
  }

  .footer-centent {

    width: 100%;
    margin: 0 auto;
    height: 63px;
    font-size: 15px;
    overflow: hidden;
  }

  .footer-centent-text {
    margin-top: 25px;
    color: white;
    text-align: center;
  }
</style>
