<template>
<div>
  <div>Hello {{ message }}</div>
  <div>Hello {{ testData }}</div>
</div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      message: 'Vue.js!!',
      testData: 'data'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
