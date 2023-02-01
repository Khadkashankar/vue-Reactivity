<script setup>
// reactivity
// import { reactive } from "vue";
import { ref } from "vue";
// let num = reactive({ a: 10, b: 20 });
// setTimeout(() => {
//   console.log("settimeout called");
//   console.log("Num", num);
//   num.a = 30;
//   console.log("a", num.a);
// }, 5000);
//ref showing sum of two numbers
let a = ref(10);
let b = ref(20);
setTimeout(() => {
  console.log("settimeout called");
  console.log("a", a);
  console.log("b", b);
  console.log("a.value", a.value);
  console.log("b.value", b.value);
  a.value = 40;
}, 5000);
//ref of count value
// let obj1 = ref({ count: 0 });
// setTimeout(() => {
//   console.log("obj1 settimeout called");
//   console.log("obj1", obj1);
//   console.log("obj1.value", obj1.value);
//   console.log("obj1.value.count", obj1.value.count);
//   obj1.value.count++;
// }, 5000);
</script>
<template>
  <!-- <h1>SUM: {{ num.a + num.b }}</h1> -->
  <h1>SUM: {{ a + b }}</h1>
  <!-- <h1>{{ obj1.count }}</h1> -->
</template>
<style scoped></style>
