<template>
  <div>
    <Navbar />
    <HeroSection />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import Navbar from '~/components/Navbar.vue';
import HeroSection from '~/components/HeroSection.vue';

export default defineComponent({
  components: {
    Navbar,
    HeroSection,
  },
});
</script>
