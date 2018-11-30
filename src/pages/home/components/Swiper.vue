<template>
<div class="wrapper">
  <swiper :options="swiperOption">
    <swiper-slide v-for="item of swiperList" :key="item.id">
      <img class="swiper-img"
           :src="item.imgUrl" />
    </swiper-slide>
    <div class="swiper-pagination"  slot="pagination"></div>
  </swiper>
  </div>
</template>
<script>

export default{
  name: 'HomeSwiper',
  data: function () {
    return {
      swiperOption: {
        pagination: '.swiper-pagination',
        loop: true
      },
      swiperList: [{
        id: '001',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1811/7c/8e5c4ab8ee8b7402.jpg_750x200_dd7a38dd.jpg'
      }, {
        id: '002',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1811/c6/2467595fffc3b302.jpg_750x200_bc88db3a.jpg'
      }, {
        id: '003',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1811/d0/bad815ec5a5e1402.jpg_750x200_b744a695.jpg'
      }, {
        id: '004',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1811/4d/6706bf772c05ce02.jpg_750x200_773e75f0.jpg'
      }
      ]
    }
  }
}
</script>
<style lang="stylus" scoped>
  .wrapper >>> .swiper-pagination-bullet
      background: #fff
  .wrapper
    overflow: hidden
    width:100%
    height:0
    padding-bottom: 26.67%
    .swiper-img
      width:100%
</style>
