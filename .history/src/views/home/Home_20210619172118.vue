<template>
  <div id="home">
    <nav-bar class="home-nav"><div slot="center">购物街</div></nav-bar>
    <swiper>
      <swiper-item v-for="item in banners" :key="item">
        <a :href="item.link"></a>
      </swiper-item>
    </swiper>
  </div>
</template>
<script>
import { getHomeMultidata } from "network/home";
import NavBar from "components/common/navbar/NavBar";
// import Swiper from "components/common/swiper/Swiper";
// import SwiperItem from "components/common/swiper/SwiperItem";
import { Swiper, SwiperItem } from "components/common/swiper/index";
export default {
  name: "Home",
  components: {
    NavBar,
    getHomeMultidata,
    Swiper,
    SwiperItem,
  },
  data() {
    return {
      banners: [],
      recommends: [],
    };
  },
  created() {
    //1.请求多个数据
    getHomeMultidata().then((res) => {
      // console.log(res);
      this.banners = res.data.banner.list;
      this.recommends = res.data.recommend.list;
      console.log(this.banners);
      console.log(this.recommends);
    });
  },
};
</script>
<style scoped>
.home-nav {
  background: var(--color-tint);
  color: white;
}
</style>
