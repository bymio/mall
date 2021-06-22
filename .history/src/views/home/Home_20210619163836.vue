<template>
  <div id="home">
    <nav-bar class="home-nav"><div slot="center">购物街</div></nav-bar>
  </div>
</template>
<script>
import { getHomeMutidata } from "network/home";
import NavBar from "components/common/navbar/NavBar";
export default {
  name: "Home",
  components: {
    NavBar,
    getHomeMutidata,
  },
  created() {
    //1.请求多个数据
    getHomeMutidata().then(res =>)
  },
};
</script>
<style scoped>
.home-nav {
  background: var(--color-tint);
  color: white;
}
</style>
