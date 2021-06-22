<template>
  <div class="category">
    <nav-bar class="category-nav">
      <div slot="center">分类</div>
    </nav-bar>

    <div class="wrapper">
      <ul>
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
    };
  },
  mounted() {
    const bscroll = new BScroll(document.querySelector(".content"), {
      probeType: 3,
      click: true,
      pullUpLoad: true,
    });

    bscroll.on("scroll", (position) => {
      // console.log(position);
    });

    bscroll.on("pullingUp", () => {
      console.log("上拉加载更多");
      // 发送网络请求, 请求更多页的数据

      // 等数据请求完成, 并且将新的数据展示出来后
      setTimeout(() => {
        bscroll.finishPullUp();
      }, 2000);
    });
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
.wrapper {
  height: 200px;
  background-color: rgb(255, 0, 0);
}
</style>
