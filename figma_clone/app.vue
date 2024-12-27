<template>
  <div>
    <Navbar />
    <MainSection />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import Navbar from '~/components/Navbar.vue';
import MainSection from './components/MainSection.vue';

export default defineComponent({
  components: {
    Navbar,
    MainSection
  },
});
</script>

<style>
* {
  font-family: Arial, sans-serif;
  /* Устанавливаем шрифт Arial глобально */
}
</style>