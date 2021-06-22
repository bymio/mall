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
import  Goods from ''
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
  methods: {},
};
</script>

<style scoped>
</style>
