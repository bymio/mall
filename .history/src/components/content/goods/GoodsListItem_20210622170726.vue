<template>
  <div class="goodsitem">
    <img :src="goodsItem.show.img" alt="" srcset="">
    <div>
      <p>{{goodsItem.title}}</p>
      <span class="price">{{goodsItem.}}</span>
      <span></span>
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
