<template>
  <div id="app">
    <header>
      <h1>Selamat Datang di Aplikasi Vue!</h1>
    </header>
    <main>
      <ParentComponent />
    </main>
    <footer>
      <p>&copy; 2023 CursorBot. Hak Cipta Dilindungi.</p>
    </footer>
  </div>
</template>

<script setup>
import ParentComponent from './components/ParentComponent.vue'
</script>

<style>
#app {
  font-family: 'Arial', sans-serif;
  text-align: center;
  margin: 0 auto;
  max-width: 800px;
  padding: 20px;
}

header {
  background-color: #080808;
  padding: 20px 0;
  border-bottom: 2px solid #131313;
}

main {
  margin-top: 20px;
}

footer {
  margin-top: 20px;
  padding: 10px 0;
  background-color: #1b1b1d;
  border-top: 2px solid #ccc;
}

button {
  background-color: #007BFF;
  color: white;
  border: none;
  padding: 10px 20px;
  border-radius: 5px;
  cursor: pointer;
  font-size: 16px;
}

button:hover {
  background-color: #0056b3;
}
</style>

