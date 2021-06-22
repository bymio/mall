<template>
  <div id="home">
    <nav-bar class="home-nav"><div slot="center">购物街</div></nav-bar>

  </div>
</template>
<script>
import { getHomeMultidata } from "network/home";
import NavBar from "components/common/navbar/NavBar";
export default {
  name: "Home",
  components: {
    NavBar,
    getHomeMultidata,
  },
  data() {
    return {
      banners:[],
      recommends:[],
    }
  },
  created() {
    //1.请求多个数据
    getHomeMultidata().then(res => {
      // console.log(res);
      this.banners = res.data.banners;
      this.recommends = res.data.recommends;
      console.log(this.banners);
      console.log(this.banners);
      
      
    })
  },
};
</script>
<style scoped>
.home-nav {
  background: var(--color-tint);
  color: white;
}
</style>
