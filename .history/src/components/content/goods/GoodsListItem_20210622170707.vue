<template>
  <div class="goodsitem">
    <img :src="goodsItem.show.img" alt="" srcset="">
    <div>
      <p>{{goodsItem.}}</p>
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
