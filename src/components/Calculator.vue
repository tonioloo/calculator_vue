<script>
  export default {
    data() {
      return {
        number1: 0,
        number2: 0,
        operation: 'add',
      };
    },
    computed: {
      result() {
        switch (this.operation) {
          case 'add':
            return this.number1 + this.number2;
          case 'subtract':
            return this.number1 - this.number2;
          case 'multiply':
            return this.number1 * this.number2;
          case 'divide':
            return this.number1 / this.number2;
          default:
            return 0;
        }
      },
    },
  };
</script>

<template>
  <div>
    <h1>Calculadora Aritimética</h1>
    <div>
      <input type="number" v-model.number="number1" placeholder="Número 1">
      <input type="number" v-model.number="number2" placeholder="Número 2">
      <select v-model="operation">
        <option value="add">+</option>
        <option value="subtract">-</option>
        <option value="multiply">*</option>
        <option value="divide">/</option>
      </select>
    </div>
    <p>Resultado: {{ result }}</p>
  </div>
</template>

<style scoped>
  div {
    margin-bottom: 10px;
  }
  input, slect {
    margin-right: 10px;
    border-radius: 50px;
    height: 22px;
  }
  input:focus {
    box-shadow: 0 0 0 0;
    outline: 0;
  }
  select {
    height: 28px;
    width: 200px;
    border-radius: 50px;
  }
</style>