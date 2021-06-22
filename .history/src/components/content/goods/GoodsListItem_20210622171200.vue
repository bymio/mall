<template>
  <div class="goods-item">
    <img :src="goodsItem.show.img" alt="" srcset="">
    <div class="goods">
      <p>{{goodsItem.title}}</p>
      <span class="price">{{goodsItem.price}}</span>
      <span class="collect">{{goodsItem.cfav}}</span>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      msg: "",
    };
  },
  props: {
    goodsItem: {
      type: Object,
      default() {
        return {};
      },
    },
  },
  methods: {},
};
</script>

<style scoped>
</style>
