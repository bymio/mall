<template>
  <div class="tab-control">
    <div class="tab-control-item" v-for="item in titles" :key="item">
      <span>
        {{ item }}
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
    titles: {
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
.tab-control {
  display: flex;
  text-align: center;
  font-size: 15px;
  height: 40px;

  line-height: 40px;
}
.tab-control-item {
  flex: 1;
}
</style>
