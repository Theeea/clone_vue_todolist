<!-- Logo + Date -->
<script setup>
import { ref, computed } from 'vue'
const timestamp = ref('')

function created() {
  const now = new Date();
  const month = now.getMonth() + 1;
  const date = now.getDate();
  const weekList = new Array("Sun.", "Mon.", "Tue.", "Wed.", "Thu.", "Fri.", "Sat.");
  const week = weekList[now.getDay()];
  timestamp.value = `${month}/${date} ${week}`;
}

const computed_timestamp = computed(
    get => created()
)
</script>

<template>
  <header class="header">
    <h1 class="logo">My Todo</h1>
    <p class="data">{{ timestamp }}</p>
  </header>
</template>
