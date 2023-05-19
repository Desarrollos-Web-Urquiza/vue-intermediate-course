<script setup lang="ts">
import { RouterView } from 'vue-router';
import Navbar from '@/shared/components/NavBar.vue';

</script>


<template>
  <div class="warapper">  
    <header>
      <Navbar 
        title="Rick and Morty"
        links=""
      />
    </header>

    <main>
      <RouterView />
    </main>
  </div>
</template>

<style scoped>

</style>
