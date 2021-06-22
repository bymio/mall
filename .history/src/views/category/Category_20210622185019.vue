<template>
  <div class="category">
    <nav-bar class="category-nav">
      <div slot="center">分类</div>
    </nav-bar>

    <div class="wrapper">
      <ul class="content">
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
        <li>222</li>
      </ul>
    </div>
  </div>
</template>

<script>
import BScroll from "better-scroll";
import NavBar from "components/common/navbar/NavBar";

export default {
  name: "Category",
  data() {
    return {
      scroll: null,
    }
  },
  mounted () {
   this.scroll = new BScroll(".wrapper", {});
  },
  components: {
    NavBar,
  },
};
</script>

<style scoped>
.category-nav {
  background: var(--color-tint);
  color: white;
}
.wrapper{
  height: 200px;
  background-color: rgb(255, 0, 0);

}
</style>
