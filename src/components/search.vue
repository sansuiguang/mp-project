<template>
  <div class="search">
    <div class="search-item">
      <icon type="search"></icon>
      <span>搜索</span>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  }
};
</script>

<style  scoped>
.search {
  padding: 20rpx;
  text-align: center;
  background-color: #eb4450;
}
.search .search-item {
  background-color: #fff;
}
.search .search-item icon {
  vertical-align: middle;
}
</style>
