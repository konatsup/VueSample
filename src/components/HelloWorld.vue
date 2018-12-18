<template>
<div>
  <div>Hello{{ user.name }}</div>
  <div>Age:{{ user.age }}</div>
  <div>Job:{{ user.job }}</div>
</div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      user: {
        name: 'デーモン閣下',
        age: 24,
        job: 'Student'
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
