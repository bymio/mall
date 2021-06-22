<template>
  <swiper>
    <swiper-item v-for="item in banners" :key="item">
      <a :href="item.link">
        <img :src="item.image" alt="" />
      </a>
    </swiper-item>
  </swiper>
</template>

<script>
import { Swiper, SwiperItem } from "components/common/swiper/index";

export default {
  data() {
    return {
      msg: "",
    };
  },
  props
  components: {
    Swiper,
    SwiperItem,
  },
  methods: {},
};
</script>

<style scoped>
</style>
