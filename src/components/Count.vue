<template>
  <div>
    <div class="text-red">{{ count }}カウント</div>
    <div class="text-blue">{{ clickCount }}クリック数</div>
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
    increment() {
      this.count += 1;
      this.clickCount += 1;
    },
    decrement() {
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
.text-red {
  color: #f22;
}
.text-blue {
  color: #22f;
}
</style>
