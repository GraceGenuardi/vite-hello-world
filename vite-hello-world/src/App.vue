

<script>
// 1. importare il componente
import AppTitle from './components/AppTitle.vue'
export default {
  components: {
    // 2. registrare il componente che abbiamo importato
    AppTitle
  },
  data() {
    return {
      message: 'La mia prima app con Vite!'
    }
  },
  methods: {
    sayHello() {
      console.log('Ciao Vite!')
    }
  }
}
</script>

<template>
  <div>
    <a href="https://vitejs.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
  </div>
  <div>
    <h1>{{ message }}</h1>
    <button @click="sayHello">Click</button>
  </div>

  <!-- 3. utilizzo il componente -->
  <AppTitle></AppTitle>


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