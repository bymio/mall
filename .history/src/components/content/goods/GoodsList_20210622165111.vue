<template>
  <div class="goods-list">
    <!-- <ul>
      <li>1</li>
      <li>1</li>
      <li>1</li>
      <li>1</li>
      <li>1</li>
      <li>1</li>
      <li>1</li>
      <li>1</li>
      <li>1</li>
      <li>1</li>
    </ul> -->
    {{ goodsList }}
  </div>
</template>

<script>
import  GoodsListItem from 'components/content/goods/GoodsListItem'
export default {
  data() {
    return {
      msg: "",
    };
  },
  prpos: {
    goodsList: {
      type: Array,
      default() {
        return [];
      },
    },
  },
  comp
  methods: {},
};
</script>

<style scoped>
</style>
