<template>
  <div class="dropdown-menu">
    <div class="columns">
      <div v-for="(column, index) in columns" :key="index" class="column">
        <ul>
          <li v-for="(item, idx) in column" :key="idx">{{ item }}</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  props: {
    columns: {
      type: Array,
      required: true,
    },
  },
});
</script>

<style scoped>
.dropdown-menu {
  position: absolute;
  background-color: white;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
}

.columns {
  display: flex;
}

.column {
  margin: 0 1rem;
}
</style>