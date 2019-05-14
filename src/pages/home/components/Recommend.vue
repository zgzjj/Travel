<template>
  <div>
    <div class="title">热销推荐</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <img class="item-img" :src="item.imgUrl"  />
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
          <button class="item-button">查看详情</button>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeRecommend',
  data () {
    return {
      recommendList: [{
        id: '001',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1612/1d/1d9a740c1f9e0efaa3.img.jpg_200x200_63285bd9.jpg',
        title: '成都海昌极地海洋公园',
        desc: '成都的标志，也是现代人对老成都的记忆'
      }, {
        id: '002',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1612/1d/1d9a740c1f9e0efaa3.img.jpg_200x200_63285bd9.jpg',
        title: '成都海昌极地海洋公园',
        desc: '成都的标志，也是现代人对老成都的记忆'
      }, {
        id: '003',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1612/1d/1d9a740c1f9e0efaa3.img.jpg_200x200_63285bd9.jpg',
        title: '成都海昌极地海洋公园',
        desc: '成都的标志，也是现代人对老成都的记忆'
      }, {
        id: '004',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1612/1d/1d9a740c1f9e0efaa3.img.jpg_200x200_63285bd9.jpg',
        title: '成都海昌极地海洋公园',
        desc: '成都的标志，也是现代人对老成都的记忆'
      }, {
        id: '005',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1612/1d/1d9a740c1f9e0efaa3.img.jpg_200x200_63285bd9.jpg',
        title: '成都海昌极地海洋公园',
        desc: '成都的标志，也是现代人对老成都的记忆'
      }, {
        id: '006',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1612/1d/1d9a740c1f9e0efaa3.img.jpg_200x200_63285bd9.jpg',
        title: '成都海昌极地海洋公园',
        desc: '成都的标志，也是现代人对老成都的记忆'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/mixins.styl'
  .title
    margin-top: .2rem
    line-height: .8rem
    background: #eee
    text-indent: .2rem
  .item
    overflow :hidden
    display :flex
    height :1.9rem
    .item-img
      width :1.7rem
      height :1.7rem
      padding :.1rem
    .item-info
      flex :1
      padding :.1rem
      min-width :0
      .item-title
        line-height :.54rem
        font-size :.32rem
        ellipse()
      .item-desc
        line-height :.4rem
        color: #ccc
        ellipse()
      .item-button
        line-height :.44rem
        margin-top: .16rem
        background :#ff9300
        padding :0 .1rem
        border-radius :.06rem
        color :#ffffff
</style>
