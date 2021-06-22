<template>
  <div class="goods-item">
    <img :src="goodsItem.show.img" alt="" srcset="" />
    <div class="goods-info">
      <p>{{ goodsItem.title }}</p>
      <span class="price">{{ goodsItem.price }}</span>
      <span class="collect">{{ goodsItem.cfav }}</span>
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
.goods-item {
  display: flex;
}
.goods-item img{
  width: 40%;
  border-radius: 5%;
}
</style>
