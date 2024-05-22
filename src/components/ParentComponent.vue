<template>
  <div>
    <ChildComponent @response="handleResponse" />
    <p>{{ message }}</p>
  </div>
</template>

<script setup>
import { ref } from 'vue'
import ChildComponent from './ChildComponent.vue'

const message = ref('Tunggu data...')

const handleResponse = (data) => {
  message.value = data
}
</script>

