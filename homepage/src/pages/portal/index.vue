<template>
  <div class="portal">
    <page-header></page-header>
    <div class="banner">
      <el-carousel :interval="5000" :height="carouselHeight" arrow="never" trigger="click">
        <el-carousel-item v-for="banner in banners" :key="banner.bid">
          <img :src="banner.imageUrl" alt="banner">
        </el-carousel-item>
      </el-carousel>
    </div>
    <div class="globalWidth">
    <!-- banner -->

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
  }
  @media screen and (min-width: 768px){
    .portal {
      .banner {
        height: 300px;
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
