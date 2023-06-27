<script setup>
import {reactive} from "vue";
  const estado = reactive({
    operad:"",
    num1: 0,
    num2: 0
  })

</script>

<template>
<div class="calculadora">
  <input type="number" placeholder="Primeiro número" v-model.number="num1">
  <select>
    <option value="+" selected> + </option>
    <option value="-"> - </option>
    <option value="*"> * </option>
    <option value="÷"> ÷ </option>
  </select>
  <input type="number" placeholder="Segundo número" v-model.number="num2">
  <h3> {{ Resultado }} </h3>
</div>

</template>

<style scoped>
</style>
