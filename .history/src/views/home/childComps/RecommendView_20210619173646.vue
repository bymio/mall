<template>
  <div class="recommends">
    <div v-for="item in recommends" :key='item'>
      <a :href="item.link">
        <img :src="item.image" alt="">
        <div>{{</div>
      </a>
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
    recommends: {
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
