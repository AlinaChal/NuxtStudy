<template>
    <div class="wraper">
     <h1>Welcome to the homepage</h1>
     <p class="p">
        Кнопка для нажатия
        <button class="b">Send</button>
     </p>
    </div>
  </template>
  
  
  <script setup lang="ts">
  </script>
  
  <style scoped lang="scss">
    :root {
      background-color: gray;
    }
    .wraper {
      background-color: bisque;
      border-radius: 1em;
      border: 5px solid #900;
      margin: 1em;
      padding: 1em;
  
      .p {
        color: blue;
  
        .b {
          color: purple;
        }
      }
    }
  </style>