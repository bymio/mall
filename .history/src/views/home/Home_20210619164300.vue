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
      resukt:null,
    }
  },
  created() {
    //1.请求多个数据
    getHomeMultidata().then(res => {
      console.log(res);
      this.result = res;
      console.log(this.result);
      
      
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
