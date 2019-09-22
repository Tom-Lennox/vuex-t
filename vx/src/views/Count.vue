<template>
  <div class="count">
    <h1>counter</h1>
    <p>vuex触る人は大体通るであろう道。</p>
    {{$store.state.count}}
    <button @click="increment">+</button>
    <button @click="decrement">-</button>
  </div>
</template>
 
<script>
export default {
  methods: {
    increment() {
      this.$store.commit("increment");
    },
    decrement() {
      this.$store.commit("decrement");
    }
  }
};
</script>
