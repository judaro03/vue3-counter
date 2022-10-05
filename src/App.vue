<script>
export default {
  data: () => ({
    contador: 0,
  }),
  methods: {
    aumentar() {
      this.contador++;
    },
    disminuir() {
      this.contador--;
    },
    reset() {
      this.contador = 0;
    },
  },
};
</script>

<template>
  <div class="container">
    <img src="./assets/logo.svg" alt="" width="125" />
    <h1>Mi primer contador</h1>
    <hr />
    <h2>Contador: {{ contador }}</h2>
    <button @click="aumentar">+1</button>
    <button @click="disminuir">-1</button>
    <button @click="reset">Reset</button>
  </div>
</template>

<style scoped>
.container {
  background-color: #ccc;
  text-align: center;
}
small {
  color: #666;
}
h1 {
  font-family: "Roboto", sans-serif;
  color: black;
  font-weight: bolder;
}
h2 {
  font-size: 2.5rem;
}
button {
  cursor: pointer;
  font-size: 1.4rem;
  margin: 0px 6px;
  background-color: #4545e6;
  color: #ccc;
  border: none;
  padding: 5px 10px;
  border-radius: 20px;
}
</style>