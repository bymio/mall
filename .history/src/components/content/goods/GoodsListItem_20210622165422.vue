<template>
  <div class="goodsitem">
    <img :src="goodsItem.show" alt="" srcset="">
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
