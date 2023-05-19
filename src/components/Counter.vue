<template>
  <h3>Counter App</h3>
  <div id="counter">
    <button type="button" class="button" @click="increment">+</button>
    <h5 class="result">Ans : {{ number }}</h5>
    <button type="button" class="button" @click="decrement">-</button>
  </div>
  <div>
    <button type="button" class="button-reset" @click="reset">RESET</button>
  </div>
</template>

<script>
export default {
  name: "CounterTab",
  data() {
    return {
      number: 0,
    };
  },
  methods: {
    increment() {
      this.number++;
    },
    decrement() {
      this.number--;
    },
    reset() {
      this.number = 0;
    },
  },
};
</script>
