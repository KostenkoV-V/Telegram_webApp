<!-- src/views/User.vue -->
<script setup>
defineProps({ id: String }) // props: true в маршруте передаёт id сюда
</script>

<template>
  <div>
    <h1>Пользователь</h1>
    <p>ID пользователя: {{ id }}</p>
  </div>
</template>
