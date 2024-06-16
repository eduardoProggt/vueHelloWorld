<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>{{ counter }}</p>
    <button @click="incrementCounter">Increase Counter</button>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return {
      counter: 0
    };
  },
  methods: {
    incrementCounter() {
      this.counter++;
    }
  }
};
</script>

<style scoped>
.hello {
  text-align: center;
  margin-top: 40px;
}
</style>
