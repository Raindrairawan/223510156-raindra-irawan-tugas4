<template>
  <div>
    <GrandchildComponent @response="handleData" />
  </div>
</template>

<script setup>
import GrandchildComponent from './GrandchildComponent.vue'
import { defineEmits } from 'vue'

const emits = defineEmits(['response'])

const handleData = (data) => {
  emits('response', data)
}
</script>

