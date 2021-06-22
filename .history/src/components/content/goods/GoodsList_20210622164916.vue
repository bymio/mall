<template>
  <div class="goods-list">
    ul
    {{ goodsList }}
  </div>
</template>

<script>
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
