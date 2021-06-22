<template>
  <div class="goodsitem">

  </div>
</template>

<script>
export default {
  data () {
    return {
      msg: ''
    }
  },
  props:{
    goodsItem:{
      type:Object,
      default(){
        return [];
      }
    }
  }
  ,
  methods: {

  }
}
</script>

<style scoped>

</style>
