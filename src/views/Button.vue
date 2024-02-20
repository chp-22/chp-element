<template>
    <button class="my-button">{{ text }}</button>
  </template>
  
  <script>
  export default {
    name: 'Button',
    props: {
      text: {
        type: String,
        default: 'Click me'
      }
    }
  }
  </script>
  
  <style scoped>
  .my-button {
    background-color: #0080ff;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 4px;
    cursor: pointer;
  }
  </style>