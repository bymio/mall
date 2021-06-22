<template>
  <div class="goods-list">
    <goods-list-item :goods-item= v-for="(item, index) in goods" :key="index">

    </goods-list-item>
    <!-- {{ goods }} -->
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
  props: {
    goods: {
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
