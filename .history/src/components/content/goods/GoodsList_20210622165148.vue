<template>
  <div class="goods-list">
    <goods-list-item></goods-list-item>
    {{ goodsList }}
  </div>
</template>

<script>
import GoodsListItem from "./GoodsListItem.vue";
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
  components: {
    GoodsListItem,
  },
  methods: {},
};
</script>

<style scoped>
</style>
