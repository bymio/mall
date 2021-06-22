<template>
  <div class="goods">
   {{goods}}
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
    goods:{
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
