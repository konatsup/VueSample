<template>
<div>
  <div>Hello{{ user.name }}</div>
  <div>Age:{{ user.age }}</div>
  <div>Job:{{ user.job }}</div>
  <div>{{todo.name}}</div>
  <input type='text' :value='todo.name' >
  <div>{{todo.name.length >=20 ? '文字数を減らしてください': ''}}</div>
</div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      user: {
        name: 'デーモン閣下',
        age: 56,
        job: 'Student'
      },
      todo: {
        name: 'あいうえおかきくけこさしすせそたちつてとな'
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
