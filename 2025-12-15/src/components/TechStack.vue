<script setup lang="ts">
interface TechItem {
  name: string;
  icon?: string;
}

interface Props {
  title: string;
  items: TechItem[];
  color?: string;
}

const props = withDefaults(defineProps<Props>(), {
  color: '#2563eb',
});
</script>

<template>
  <div class="tech-stack">
    <h3 class="tech-title" :style="{ borderColor: props.color }">
      {{ props.title }}
    </h3>
    <ul class="tech-list">
      <li v-for="(item, index) in props.items" :key="index" class="tech-item">
        <span v-if="item.icon" class="tech-icon">{{ item.icon }}</span>
        <span class="tech-name">{{ item.name }}</span>
      </li>
    </ul>
  </div>
</template>

<style scoped>
.tech-stack {
  padding: 1.5rem;
}

.tech-title {
  font-size: 1.5rem;
  font-weight: 700;
  margin-bottom: 1.5rem;
  padding-bottom: 0.75rem;
  border-bottom: 3px solid;
  color: #1e293b;
}

.tech-list {
  list-style: none;
  padding: 0;
  margin: 0;
  display: flex;
  flex-direction: column;
  gap: 0.75rem;
}

.tech-item {
  display: flex;
  align-items: center;
  gap: 0.75rem;
  font-size: 1.1rem;
  color: #334155;
  padding: 0.5rem 0;
}

.tech-icon {
  font-size: 1.5rem;
  width: 2rem;
  display: inline-flex;
  justify-content: center;
}

.tech-name {
  font-weight: 500;
}
</style>
