<template>
  <div>
    <div class="title">热销推荐</div>
    <ul>
      <li class="item border-bottom"
          v-for="item of recommendList"
          :key="item.id">
          <img class="item-img" :src="item.imgUrl" />
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
          <button class="item-botton">查看详情</button>
        </div>
      </li>
    </ul>
  </div>
</template>
<script>
export default{
  name: 'HomeRecommend',
  data: function () {
    return {
      recommendList: [{
        id: '0001',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1811/d4/d4a663613604238ea3.img.jpg_200x200_b412a8a2.jpg',
        title: '长隆野生动物世界',
        desc: '熊猫三胞胎与您共享欢乐时光'
      }, {
        id: '0002',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1811/e0/e0a9c262bb657ee9a3.img.jpg_200x200_0b1847a6.jpg',
        title: '长隆国际大马戏剧院',
        desc: '跟着大马戏团一起party~'
      }, {
        id: '0003',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1809/56/5639ccfd58c4cca4a3.img.png_200x200_0027165c.png',
        title: '广州正佳极地海洋世界',
        desc: '梦幻主题式极地海洋体验'
      }]
    }
  }
}
</script>
<style lang="stylus" scoped>
  @import '~styles/mixins.styl'
  .title
    margin-top: .2rem
    line-height:.8rem
    background:#eee
    text-indent:.2rem
  .item
    display: flex
    overflow: hidden
    height:1.9rem
    .item-img
      width:1.7rem
      height:1.7rem
      padding:.1rem
    .item-info
      flex:1
      padding:.1rem
      min-width:0
      .item-title
        line-height:.54rem
        font-size:.32rem
        ellipsis()
      .item-desc
        line-height:.4rem
        color:#ccc
        ellipsis()
      .item-botton
        line-height:.44rem
        margin-top:.16rem
        background: #ff9300
        padding: 0 .1rem
        border-radius: .06rem
        color:#fff
</style>
