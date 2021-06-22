<template>
  <div class="goods-list">
    <goods-list-item v-for="(item, index) in goodsList" :key="index"></goods-list-item>
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
