<template>
  <div class="wrapper">
    <swiper :options="swiperOption">
      <!-- slides -->
      <swiper-slide v-for="item in swiperList" :key="item.id">
        <img class="swiper-img" :src="item.imgUrl"/>
      </swiper-slide>
      <!-- Optional controls -->
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
      swiperList: [{
        id: '001',
        imgUrl: 'https://img1.qunarzz.com/vc/b8/25/51/f6173dbd12c1a0f783abe73855.jpg'
      }, {
        id: '002',
        imgUrl: 'https://img1.qunarzz.com/vc/bf/9d/a3/67b7b37511fa26a78298bf1da1.jpg'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  .wrapper >>> .swiper-pagination-bullet-active
    background :#fff !important
  .wrapper
    overflow :hidden;
    background :#eee;
    width :100%;
    height :0;
    padding-bottom :31.25%;
    .swiper-img
      width: 100%
</style>
