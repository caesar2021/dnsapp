<template>
  <label class="mb-1 text-sm font-semibold" v-text="title"></label>
</template>

<script setup>

import { defineProps } from 'vue'

defineProps({
  title: String
})

</script>