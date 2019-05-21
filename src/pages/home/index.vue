<template>
  <div>
    <search-bar/>
    <!-- 轮播图部分 -->
    <swiper :indicator-dots="indicatorDots">
      <swiper-item :key="index" v-for="(item,index) in imgUrls">
        <image :src="item" class="slide-image"/>
      </swiper-item>
    </swiper>
  </div>
</template>

<script>
// 导入公共的search组件
import SearchBar from "../../components/search";
export default {
  data() {
    return {
      //该属性的作用显示轮播图小圆点
      indicatorDots: true,
      imgUrls: [
        "https://images.unsplash.com/photo-1551334787-21e6bd3ab135?w=640",
        "https://images.unsplash.com/photo-1551214012-84f95e060dee?w=640",
        "https://images.unsplash.com/photo-1551446591-142875a901a1?w=640"
      ]
    };
  },
  components: {
    "search-bar": "SearchBar"
  }
};
</script>

<style  scoped>
.slide-image {
  width: 750rpx;
}
</style>
