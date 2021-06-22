<template>
  <div class="category">
    <nav-bar class="category-nav">
      <ul>
        
      </ul>
    </nav-bar>
  </div>
</template>

<script>
import NavBar from "components/common/navbar/NavBar";

export default {
  name: "Category",
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
</style>
