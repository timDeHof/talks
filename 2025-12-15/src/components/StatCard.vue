<script setup lang="ts">
interface Props {
  percentage: string;
  icon: string;
  description: string;
  color?: string;
}

const props = withDefaults(defineProps<Props>(), {
  color: '#2563eb',
});
</script>

<template>
  <div class="stat-card">
    <div class="stat-percentage" :style="{ color: props.color }">
      {{ props.percentage }}
    </div>
    <div class="stat-icon">
      <i :class="props.icon" :style="{ color: props.color }"></i>
    </div>
    <div class="stat-description">
      {{ props.description }}
    </div>
  </div>
</template>

<style scoped>
.stat-card {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 2rem;
  text-align: center;
  gap: 1rem;
}

.stat-percentage {
  font-size: 4rem;
  font-weight: 700;
  line-height: 1;
}

.stat-icon {
  font-size: 3.5rem;
  opacity: 0.9;
}

.stat-description {
  font-size: 1.1rem;
  color: #334155;
  line-height: 1.5;
  max-width: 300px;
}
</style>
