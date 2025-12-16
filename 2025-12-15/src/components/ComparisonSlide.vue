<script setup lang="ts">
interface Props {
  leftTitle: string;
  rightTitle: string;
  leftItems: string[];
  rightItems: string[];
  leftColor?: string;
  rightColor?: string;
}

const props = withDefaults(defineProps<Props>(), {
  leftColor: '#dc2626',
  rightColor: '#16a34a',
});
</script>

<template>
  <div class="comparison-container">
    <div class="comparison-side left">
      <h3 class="comparison-title" :style="{ color: props.leftColor }">
        {{ props.leftTitle }}
      </h3>
      <ul class="comparison-list">
        <li
          v-for="(item, index) in props.leftItems"
          :key="index"
          class="comparison-item"
        >
          <span
            class="bullet"
            :style="{ backgroundColor: props.leftColor }"
          ></span>
          {{ item }}
        </li>
      </ul>
    </div>

    <div class="divider">
      <svg width="60" height="200" viewBox="0 0 60 200" class="arrow-curve">
        <defs>
          <linearGradient id="gradient" x1="0%" y1="0%" x2="100%" y2="0%">
            <stop offset="0%" :style="{ stopColor: props.leftColor }" />
            <stop offset="100%" :style="{ stopColor: props.rightColor }" />
          </linearGradient>
        </defs>
        <path
          d="M 10 100 Q 30 150, 50 100"
          stroke="url(#gradient)"
          stroke-width="3"
          fill="none"
          marker-end="url(#arrowhead-comparison)"
        />
        <marker
          id="arrowhead-comparison"
          markerWidth="10"
          markerHeight="10"
          refX="9"
          refY="3"
          orient="auto"
        >
          <polygon points="0 0, 10 3, 0 6" :fill="props.rightColor" />
        </marker>
      </svg>
    </div>

    <div class="comparison-side right">
      <h3 class="comparison-title" :style="{ color: props.rightColor }">
        {{ props.rightTitle }}
      </h3>
      <ul class="comparison-list">
        <li
          v-for="(item, index) in props.rightItems"
          :key="index"
          class="comparison-item"
        >
          <span
            class="bullet"
            :style="{ backgroundColor: props.rightColor }"
          ></span>
          {{ item }}
        </li>
      </ul>
    </div>
  </div>
</template>

<style scoped>
.comparison-container {
  display: grid;
  grid-template-columns: 1fr auto 1fr;
  gap: 2rem;
  align-items: center;
  padding: 2rem;
}

.comparison-side {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}

.comparison-title {
  font-size: 1.5rem;
  font-weight: 700;
  margin: 0;
  line-height: 1.3;
}

.comparison-list {
  list-style: none;
  padding: 0;
  margin: 0;
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.comparison-item {
  display: flex;
  align-items: flex-start;
  gap: 0.75rem;
  font-size: 1.1rem;
  color: #334155;
  line-height: 1.5;
}

.bullet {
  width: 8px;
  height: 8px;
  border-radius: 50%;
  margin-top: 0.5rem;
  flex-shrink: 0;
}

.divider {
  display: flex;
  align-items: center;
  justify-content: center;
}

.arrow-curve {
  opacity: 0.7;
}
</style>
