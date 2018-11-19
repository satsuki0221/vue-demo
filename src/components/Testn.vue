<template>
  <div class="box">
    aaa: {{ count }}
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    count: Number
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.box {
  margin: 20px;
}
</style>
