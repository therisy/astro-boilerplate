<template>
    <div class="flex flex-col items-center">
      <div>Vue Count: {{ count }}</div>
      <div class="flex gap-4">
        <button @click="subtract">-</button>
        <button @click="add">+</button>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "CounterVue",
    data() {
      return {
        count: 0,
      };
    },
    methods: {
      add() {
        this.count++;
      },
      subtract() {
        this.count--;
      },
    },
  };
  </script>
  
  <style scoped>
  
  </style>