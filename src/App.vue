<script>
export default {
  // data() {
  //   return {
  //     contador: 200,
  //   };
  // },
  data: () => ({
    contador: 0,
  }),
  methods: {
    aumentar() {
      //this.contador = this.contador + 1;
      this.contador++;
    },
    disminuir() {
      //this.contador = this.contador - 1;
      this.contador--;
    },
    reset() {
      this.contador = 0;
    },
  },
};
</script>

<template>
  <article class="containter">
    <img src="./assets/logo.svg" alt="logo" width="200" />
    <h1>Hola</h1>
    <hr />
    <h2>Contador: {{ contador }}</h2>
    <button @click="aumentar()">+1</button>
    <button @click="disminuir()">-1</button>
    <button @click="reset()">Reset</button>
  </article>
</template>

<style scoped>
.containter {
  background: pink;
}
</style>