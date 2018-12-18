<template>
  <div>
    <div>{{ count }}回クリック</div>
    <button v-on:click="increment">カウントを増やす</button>
    <div class="counter">Count</div>
  </div>
</template>

<script>
export default {
  name: "Count",
  data() {
    return {
      count: 0
    };
  },
  methods: {
    increment: function() {
      this.count += 1;
    }
  }
};
</script>

<style scoped>
.counter {
  font-size: 26px;
  background-color: #dfd;
}
</style>
