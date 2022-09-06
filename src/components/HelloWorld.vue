<script setup lang="ts">
import { ref, computed, defineProps } from 'vue';

const props = defineProps({
  color: String,
});

const tc = computed(() => `bg-[${props.color}]`);
</script>

<template>
  <div class="w-[100px] h-[100px]">
    {{ tc }}
  </div>
</template>

<style scoped></style>
