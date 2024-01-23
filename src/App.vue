<script>
export default {
  data: () => ({
    counter: 10
  }),
  methods: {
    increment() {
      this.counter++
    },
    decrement() {
      this.counter--
    },
    reset() {
      this.counter = 10
    }
  }
}
</script>

<template>
  <div class="container">
    <img alt="Vue logo" src="./assets/logo.svg" width="125" height="125" />
    <small>
      <h1>Hola Mundo desde Vue 3 Javi</h1>
    </small>
    <hr />

    <h2>Contador: {{ counter }}</h2>
    <button @click="increment()">+1</button>
    <button @click="decrement()">-1</button>
    <button @click="reset()">Reset</button>
  </div>
</template>

<style scoped>
.container {
  text-align: center;
}

small {
  color: #666666;
}

h1 {
  font-weight: bolder;
}

h2 {
  font-size: 2.5rem;
}

button {
  cursor: pointer;
  font-size: 1.5rem;
  margin: 0px 5px;
}
</style>
