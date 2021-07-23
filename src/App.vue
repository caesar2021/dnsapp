<template>
  <div class="text-gray-700">
    <zb-dns-form classes="px-2">
      <zb-input-text label="Hostname"/>
      <zb-select label="Domain" :options="state.domains"/>
    </zb-dns-form>
  </div>
</template>

<script setup>
  import { reactive } from 'vue'
  import ZbDnsForm from './components/Form.vue'
  import ZbInputText from './components/InputText.vue'
  import ZbSelect from './components/Select.vue'

  const state = reactive({
    domains: [
      '.google.com',
      '.facebook.com'
    ]
  })

</script>