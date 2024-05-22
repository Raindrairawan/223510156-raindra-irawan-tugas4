<template>
  <div>
    <input v-model="userData" placeholder="Masukkan data baru..." />
    <button @click="sendData">Kirim Data</button>
  </div>
</template>

<script setup>
import { ref, defineEmits } from 'vue'

const userData = ref('')
const emits = defineEmits(['response'])

const sendData = () => {
  emits('response', userData.value)
  userData.value = ''  // Reset input setelah data terkirim
}
</script>

