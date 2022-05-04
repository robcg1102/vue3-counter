<script>
export default {
  data: () => ({
    contador: 0,
  }),
  methods: {
    incrementar() {
      this.contador++
    },
    disminuir(){
      this.contador--
    },
    reset(){
      this.contador = 0
    }
  },
};
</script>

<template>
  <div class="container">
    <img src="./assets/logo.svg" alt="" width="125" />
    <small>
      <h1>Hola Mundo</h1>
    </small>
    <hr />
    <h2>Contador: {{ contador }}</h2>
    <button @click="incrementar()">+1</button>
    <button @click="disminuir()">-1</button>
    <button @click="reset()">Reset</button>
  </div>
</template>

<style scoped>
small {
  color: #666;
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
  margin: 0 6px;
}

.container {
  text-align: center;
}
</style>
