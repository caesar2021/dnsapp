<template>
  <form :class="classes" method="POST">
    <slot/>
    <button type="submit" class="bg-green-500 text-white py-3 px-10 rounded">SUBMIT</button>
  </form>
</template>

<script setup>
  import { defineProps } from 'vue'

  defineProps({
    classes: String,
  })


</script>