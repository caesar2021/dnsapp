<template>
  <div class="flex flex-col mb-2">
    <zb-label :title="label"/>
    <select class="p-2 border border-gray-300 rounded" v-model="state.value">
      <option v-for="item in options" :value="item">{{ item }}</option>
    </select>
  </div>
</template>

<script setup>
  import { defineProps, reactive } from 'vue'
  import ZbLabel from './FormLabel.vue'

  defineProps({
    label: String,
    options: Array
  })

  const state = reactive({
    value: ''
  })

</script>