<template>
  <div class="tab-control">
    <div v-for="item in titles" :key="item">
      <span>
        {{item}}
      </span>
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
    title: {
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
