<template>
    <div class="wrapper">
        <swiper :options="swiperOption">
        <swiper-slide v-for="item of swiperList" :key="item.id">
            <img class="swipe-img" :src="item.imgSrc">
        </swiper-slide>
        <div class="swiper-pagination"  slot="pagination"></div>
    </swiper>
    </div>
</template>

<script>
export default {
  name: 'HomeSwiper',
  data () {
    return {
      swiperOption: {
        pagination: '.swiper-pagination',
        loop: true
      },
      swiperList: [
        {
          id: '001',
          imgSrc: 'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20201/9c4bd16baa22bcd6810b714b225b5c33.jpg_750x200_95d6ad38.jpg'
        },
        {
          id: '002',
          imgSrc: 'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20201/8c458e9fe5b5f4575b1d7ec0489a9ff8.jpg_750x200_f0fbf511.jpg'
        }
      ]
    }
  }
}
</script>

<style lang="stylus" scoped>
    .wrapper >>> .swiper-pagination-bullet-active
        background #fff
    .wrapper
        width 100%
        height 0
        overflow hidden
        padding-bottom 31.25%
        .swipe-img
            width 100%
</style>
