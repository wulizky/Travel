<template>
  <ul class="list">
<<<<<<< HEAD
    <li class="item">A</li>
    <li class="item">A</li>
    <li class="item">A</li>
    <li class="item">A</li>
    <li class="item">A</li>
    <li class="item">A</li>
    <li class="item">A</li>
    <li class="item">A</li>
    <li class="item">A</li>

=======
    <li class="item"
        v-for="(item,key) of cities"
        :key="key">
        {{key}}
     </li>
>>>>>>> city-ajax
  </ul>
</template>

<script>
export default{
<<<<<<< HEAD
  name: 'CityAlphabet'
=======
  name: 'CityAlphabet',
  props: {
    cities: Object
  }
>>>>>>> city-ajax
}
</script>

<style lang="stylus" scoped>
  @import '~styles/variables.styl'
  .list
    display:flex
    flex-direction:column
    justify-content:center
    position:absolute
    top:1.58rem
    right:0
    bottom:0
    width:.4rem
    .item
      line-height:.4rem
      text-align:center
<<<<<<< HEAD
      color:$bgcolor

=======
      color:$bgColor
>>>>>>> city-ajax
</style>
