<template>
  <div>
    <page-header></page-header>
    <div class="wrapper">
      <h2 class="header-title">
        关于我们
      </h2>
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
    .header-title {
      background: red;
    }
  }
</style>
