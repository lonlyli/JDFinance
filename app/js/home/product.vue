<template>
  <Panel :class="$style.panel" title="新品推荐">
    <section :class="$style.content">
      <div class="arrow">更多尖货 ></div>
      <Slider :options="options" :items="items" cname="product-slider"/>
    </section>
  </Panel>
</template>

<script>
import Panel from '../core/panel.vue'
import Slider from '../core/slider.vue'
export default {
  components: {
    Panel,
    Slider,
  },

  data() {
    return {
      items: [{
        href: 'home',
        src: '//img12.360buyimg.com/jrpmobile/jfs/t13963/267/2355123229/48850/254f797a/5a3c59aeN9cb550f6.jpg?width=335&height=421',
      }, {
        href: 'home',
        src: '//img12.360buyimg.com/jrpmobile/jfs/t13021/306/1996997425/21953/bda69db3/5a2f6a17N9da099b1.jpg?width=335&height=421',
      }, {
        href: 'home',
        src: '//img12.360buyimg.com/jrpmobile/jfs/t14125/310/1997192193/46667/3c910f8b/5a2f6a36Nad95b650.jpg?width=335&height=421',
      }, {
        href: 'home',
        src: '//img12.360buyimg.com/jrpmobile/jfs/t1/23341/11/9773/8559/5c81cde2E0192b8d3/0f158693fe9da2b8.jpg?width=335&height=421',
      }],
      options: {
        slidesPerView: 2.3,
        spaceBetween: 30,
        freeMode: true,
      },
    }
  },

}
</script>

<style lang='scss' module>
@import "../../css/element.scss";
.panel{
  @include panel;
  .content{
    padding-bottom: 40px;
    position: relative;
    >div{
      position: absolute;
      font-size: 28px;
      color: #999;
      right: 20px;
      top: -75px;
    }
  }
}
</style>
