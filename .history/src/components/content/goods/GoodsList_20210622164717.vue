<template>
  <div class="goodslist">
   {{goodsList}}
  </div>
</template>

<script>
export default {
  data () {
    return {
      msg: ''
    }
  },
  prpos:{
    goodsList:{
      type:Array,
      default(){
        return [];
      }
    }
  },
  methods: {

  }
}
</script>

<style scoped>

</style>
