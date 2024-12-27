<template>

  <section class="hero-section">
    <span class="hero">

      <img src="@/public/Hero_Img.png" alt="Hero" />
      <button class="get-started-animated">Get started for free <span class="arrow">→</span></button>

    </span>
  </section>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({});
</script>

<style scoped>
.hero img {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
}

.get-started-animated {
  position: relative;
  transition: transform 0.3s;
}

.get-started-animated:hover {
  transform: scale(1.05);
}

.arrow {
  margin-left: 0.5rem;
}
</style>