<!-- Welcome msg, task cnt -->
<script setup>
  import {ref} from 'vue'

  const title_data = ref({
    message: 'Hello, guest',
    taskTotal: 5
  })
</script>

<template>
  <div class="title">
    <p class="title__message">{{ title_data.message }}</p>
    <p class="title__task">
      You've got
      <span class="title__task-total">{{ title_data.taskTotal }}</span> tasks today.
    </p>
  </div>
</template>