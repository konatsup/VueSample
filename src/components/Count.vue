<template>
  <div>
    <div>{{ count }}カウント</div>
    <div>{{ clickCount }}クリック数</div>
    <button v-on:click="increment">カウントを増やす</button>
    <button v-on:click="decrement">カウントを減らす</button>
    <div class="counter">Count</div>
  </div>
</template>

<script>
export default {
  name: "Count",
  data() {
    return {
      count: 0,
      clickCount: 0
    };
  },
  methods: {
    increment: function() {
      this.count += 1;
      this.clickCount += 1;
    },
    decrement: function() {
      this.count -= 1;
      this.clickCount += 1;
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
