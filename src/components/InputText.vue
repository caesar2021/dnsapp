<template>
  <div class="flex flex-col mb-2">
    <zb-label :title="label"/>
    <input type="text" class="p-2 border border-gray-300 rounded" v-model="state.value"/>
  </div>
</template>

<script setup>
  import { defineProps, reactive } from 'vue'
  import ZbLabel from './FormLabel.vue'
  defineProps({
    label: String
  })
  const state = reactive({
    value: ""
  })
</script>