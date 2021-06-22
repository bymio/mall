<template>
  <div id="home">
    <nav-bar class="home-nav"><div slot="center">购物街</div></nav-bar>

  </div>
</template>
<script>
import { getHomeMultidata } from "network/home";
import NavBar from "components/common/navbar/NavBar";
// import Swiper from "components/common/swiper/Swiper";
// import SwiperItem from "components/common/swiper/SwiperItem";
export default {
  name: "Home",
  components: {
    NavBar,
    getHomeMultidata,
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
      this.banners = res.data.banner.list;
      this.recommends = res.data.recommend.list;
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
