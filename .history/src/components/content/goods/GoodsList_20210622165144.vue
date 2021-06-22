<template>
  <div class="goods-list">
    goods
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
