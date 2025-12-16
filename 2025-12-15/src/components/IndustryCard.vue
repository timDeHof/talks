<script setup lang="ts">
interface Props {
  title: string;
  icon: string;
  description: string;
  color?: string;
}

const props = withDefaults(defineProps<Props>(), {
  color: '#2563eb',
});
</script>

<template>
  <div class="industry-card">
    <div class="industry-icon" :style="{ color: props.color }">
      <i :class="props.icon"></i>
    </div>
    <h4 class="industry-title">{{ props.title }}</h4>
    <p class="industry-description">{{ props.description }}</p>
  </div>
</template>

<style scoped>
.industry-card {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  padding: 2rem 1.5rem;
  gap: 1rem;
  background: white;
  border-radius: 0.5rem;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.1);
  transition:
    transform 0.2s,
    box-shadow 0.2s;
}

.industry-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
}

.industry-icon {
  font-size: 3rem;
  line-height: 1;
}

.industry-title {
  font-size: 1.3rem;
  font-weight: 700;
  color: #1e293b;
  margin: 0;
}

.industry-description {
  font-size: 1rem;
  color: #64748b;
  line-height: 1.6;
  margin: 0;
}
</style>
