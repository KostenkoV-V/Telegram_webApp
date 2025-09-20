<script setup>
import HelloWorld from './components/HelloWorld.vue'
</script>


<template>
  <div>
    <nav>
      <router-link to="/">Главная</router-link> |
      <router-link to="/about">О сайте</router-link> |
      <router-link :to="{ name: 'User', params: { id: 42 } }">Пользователь 42</router-link>
    </nav>

    <hr />

  
    <router-view />
  </div>
</template>


<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
