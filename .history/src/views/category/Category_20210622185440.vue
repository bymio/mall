<template>
  <div class="category">
    <nav-bar class="category-nav">
      <div slot="center">分类</div>
    </nav-bar>
  </div>
</template>

<script>
import NavBar from "components/common/navbar/NavBar";

export default {
  name: "Category",
  data() {
    return {
    }
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
