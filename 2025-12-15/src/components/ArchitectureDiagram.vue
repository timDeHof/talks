<template>
  <div class="architecture-diagram">
    <svg viewBox="0 0 800 400" xmlns="http://www.w3.org/2000/svg">
      <!-- Client -->
      <g class="node">
        <rect x="50" y="170" width="120" height="60" rx="5" class="node-rect" />
        <text x="110" y="205" class="node-text">Client</text>
        <text x="110" y="220" class="node-subtext">(Web/Mobile)</text>
      </g>

      <!-- Arrow 1 -->
      <path
        d="M 170 200 L 230 200"
        class="arrow"
        marker-end="url(#arrowhead)"
      />

      <!-- API Gateway -->
      <g class="node">
        <rect
          x="230"
          y="170"
          width="120"
          height="60"
          rx="5"
          class="node-rect"
        />
        <text x="290" y="205" class="node-text">API Gateway</text>
      </g>

      <!-- Arrow 2 -->
      <path
        d="M 350 200 L 410 200"
        class="arrow"
        marker-end="url(#arrowhead)"
      />

      <!-- Microservices Container -->
      <g class="microservices">
        <rect
          x="410"
          y="80"
          width="180"
          height="240"
          rx="5"
          class="container-rect"
        />
        <text x="500" y="105" class="container-label">Microservices</text>

        <!-- Service 1 -->
        <rect
          x="430"
          y="120"
          width="140"
          height="45"
          rx="3"
          class="service-rect"
        />
        <text x="500" y="147" class="service-text">User Service</text>

        <!-- Service 2 -->
        <rect
          x="430"
          y="177"
          width="140"
          height="45"
          rx="3"
          class="service-rect"
        />
        <text x="500" y="204" class="service-text">Order Service</text>

        <!-- Service 3 -->
        <rect
          x="430"
          y="234"
          width="140"
          height="45"
          rx="3"
          class="service-rect"
        />
        <text x="500" y="261" class="service-text">Inventory Service</text>
      </g>

      <!-- Arrow 3 -->
      <path
        d="M 590 200 L 650 200"
        class="arrow"
        marker-end="url(#arrowhead)"
      />

      <!-- Database -->
      <g class="node">
        <ellipse cx="710" cy="185" rx="60" ry="30" class="db-ellipse" />
        <ellipse cx="710" cy="185" rx="60" ry="10" class="db-top" />
        <line x1="650" y1="185" x2="650" y2="215" class="db-line" />
        <line x1="770" y1="185" x2="770" y2="215" class="db-line" />
        <ellipse cx="710" cy="215" rx="60" ry="10" class="db-bottom" />
        <text x="710" y="240" class="node-text">Database</text>
        <text x="710" y="255" class="node-subtext">(SQL/NoSQL)</text>
      </g>

      <!-- Load Testing Badge -->
      <g class="badge">
        <rect
          x="620"
          y="30"
          width="140"
          height="35"
          rx="17.5"
          class="badge-rect"
        />
        <text x="690" y="52" class="badge-text">Load Testing</text>
      </g>

      <!-- Arrow marker definition -->
      <defs>
        <marker
          id="arrowhead"
          markerWidth="10"
          markerHeight="10"
          refX="9"
          refY="3"
          orient="auto"
        >
          <polygon points="0 0, 10 3, 0 6" fill="#2563eb" />
        </marker>
      </defs>
    </svg>
  </div>
</template>

<style scoped>
.architecture-diagram {
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

svg {
  max-width: 100%;
  height: auto;
}

.node-rect {
  fill: #dbeafe;
  stroke: #2563eb;
  stroke-width: 2;
}

.container-rect {
  fill: #f0f9ff;
  stroke: #2563eb;
  stroke-width: 2;
  stroke-dasharray: 5, 5;
}

.service-rect {
  fill: #bfdbfe;
  stroke: #1e40af;
  stroke-width: 1.5;
}

.db-ellipse {
  fill: #dbeafe;
  stroke: #2563eb;
  stroke-width: 2;
}

.db-top,
.db-bottom {
  fill: #93c5fd;
  stroke: #2563eb;
  stroke-width: 2;
}

.db-line {
  stroke: #2563eb;
  stroke-width: 2;
}

.badge-rect {
  fill: #f59e0b;
  stroke: #d97706;
  stroke-width: 2;
}

.node-text {
  font-size: 16px;
  font-weight: 600;
  fill: #1e40af;
  text-anchor: middle;
}

.node-subtext {
  font-size: 12px;
  fill: #64748b;
  text-anchor: middle;
}

.container-label {
  font-size: 14px;
  font-weight: 600;
  fill: #1e40af;
  text-anchor: middle;
}

.service-text {
  font-size: 13px;
  font-weight: 500;
  fill: #1e40af;
  text-anchor: middle;
}

.badge-text {
  font-size: 14px;
  font-weight: 600;
  fill: white;
  text-anchor: middle;
}

.arrow {
  stroke: #2563eb;
  stroke-width: 2;
  fill: none;
}
</style>
