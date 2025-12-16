---
theme: seriph
background: /backgrounds/hero-split.png
class: text-center
highlighter: shiki
lineNumbers: false
info: |
  ## Engineering Software Integrity
  A presentation by Timothy DeHof on applying engineering principles to software development.
drawings:
  persist: false
transition: slide-left
title: Engineering Software Integrity
mdc: true
---

<div class="bg-black py-4 opacity-85 w-full">
  <h1 class="font-medium">Is your software just <span class="font-bold font-italic">built</span>, <br/>or is it <span class="font-bold font-italic">engineered</span> ?</h1>
  <p>In a world of fast features, the most valuable asset is engineered robustness.</p>
</div>

---

layout: two-cols
background: /backgrounds/blueprint-texture.png

---

<template v-slot:default>

# From Physical Systems to Digital Architecture.

## Modern Architecture

<ArchitectureDiagram class="mt-8" />

</template>

<template v-slot:right>

## Introduction

**Timothy DeHof**: A Full-Stack Engineer with a B.S. in Mechanical Engineering. This isn't a career change; it's the fusion of two disciplines dedicated to one goal: building systems that are reliable, scalable, and maintainable for the long term.

### Key Focus

Building systems with engineering precision applied to software development.

</template>

---

layout: default
background: /backgrounds/grid-technical.png

---

# An Engineer's Mindset for Software Integrity

<div class="text-center mb-8 text-xl">
If software is a machine, an engineer understands its core principles:
</div>

<div class="grid grid-cols-2 gap-12 px-8">

<div class="space-y-4">

### Physical Engineering

<div class="flex items-start gap-3 p-3 bg-blue-50 rounded">
  <span class="text-2xl">⚙️</span>
  <div>
    <strong>Bill of Materials</strong> → Dependency Management & Supply Chain Security
  </div>
</div>

<div class="flex items-start gap-3 p-3 bg-blue-50 rounded">
  <span class="text-2xl">📏</span>
  <div>
    <strong>Tolerances</strong> → Error Handling & Graceful Degradation
  </div>
</div>

<div class="flex items-start gap-3 p-3 bg-blue-50 rounded">
  <span class="text-2xl">🔍</span>
  <div>
    <strong>Failure Analysis</strong> → Rigorous Debugging & Systemic QA
  </div>
</div>

<div class="flex items-start gap-3 p-3 bg-blue-50 rounded">
  <span class="text-2xl">🔧</span>
  <div>
    <strong>Maintenance Cycles</strong> → Long-Term Code Maintainability
  </div>
</div>

</div>

<div class="flex items-center justify-center">
  <ArchitectureDiagram />
</div>

</div>

---

layout: two-cols
background: /backgrounds/grid-technical.png

---

<template v-slot:default>

# Forged in High-Stakes Environments.

<div class="space-y-4">

### Professional Background

**7+ years** as a Mechanical Design Engineer at Polyhistor International, serving highly regulated industries.

<div class="grid grid-cols-2 gap-4 mt-6">
  <div class="text-center p-4 bg-white rounded shadow">
    <div class="text-4xl mb-2">🏥</div>
    <div class="font-bold">Medical</div>
  </div>
  <div class="text-center p-4 bg-white rounded shadow">
    <div class="text-4xl mb-2">🛡️</div>
    <div class="font-bold">Defense</div>
  </div>
  <div class="text-center p-4 bg-white rounded shadow">
    <div class="text-4xl mb-2">🖨️</div>
    <div class="font-bold">3D Printing</div>
  </div>
  <div class="text-center p-4 bg-white rounded shadow">
    <div class="text-4xl mb-2">✅</div>
    <div class="font-bold">QA</div>
  </div>
</div>

</div>

</template>

<template v-slot:right>

### Key Achievements

<div class="space-y-3 text-lg">

- Led over **30 3D printing projects** for **Medical and Defense** clients.

- Expertise in rigorous QA, defect detection, and uncompromising adherence to specifications.

- Automated internal quoting tools with Python & SQL, reducing time by **50%**.

</div>

</template>

---

layout: center
class: text-center
background: /backgrounds/grid-technical.png

---

# The Engineering Discipline Applied to Code

<div class="grid grid-cols-3 gap-8 mt-12 px-12">

<StatCard
  percentage="25%"
  icon="i-mdi-cube-outline"
  description="Accelerated front-end development cycle through modular architecture."
  color="#2563eb"
/>

<StatCard
  percentage="99.9%"
  icon="i-mdi-shield-check"
  description="Maintained service reliability for a scalable SaaS platform."
  color="#16a34a"
/>

<StatCard
  percentage="30%"
  icon="i-mdi-rocket-launch"
  description="Faster production deployments via CI/CD pipeline optimization."
  color="#f59e0b"
/>

</div>

---

layout: two-cols
background: /backgrounds/grid-technical.png

---

<template v-slot:default>

# Architecting an Enterprise-Ready SaaS Frontend

## Architecture Pattern

<div class="mt-6 space-y-4">

```mermaid
graph TD
    A[Modular Component Library<br/>TypeScript] --> B[Tenant App A]
    A --> C[Tenant App B]
    A --> D[Tenant App C<br/>✓ WCAG 2.1]

    style A fill:#dbeafe,stroke:#2563eb
    style B fill:#f0f9ff,stroke:#0284c7
    style C fill:#f0f9ff,stroke:#0284c7
    style D fill:#dcfce7,stroke:#16a34a
```

</div>

</template>

<template v-slot:right>

## Key Achievements

<div class="space-y-4">

**Modular Component Library**: Architected and deployed in TypeScript, establishing a single source of truth.

**Scalable Multi-Tenant Design**: Ensured code was reusable, maintainable, and could serve multiple customers securely.

**Accessibility by Design**: Ensured full **WCAG 2.1 accessibility compliance** in customer dashboards, a non-negotiable for enterprise readiness.

Mentored team on Test-Driven Development (TDD), improving code quality metrics by **20%**.

</div>

</template>

---

layout: center
class: text-center
background: /backgrounds/grid-technical.png

---

# Validated by the Development Community

<div class="mt-8">

## Open Source: Shadcn Timeline Component Library

<div class="grid grid-cols-2 gap-12 mt-8 max-w-3xl mx-auto">

<div class="p-8 bg-white rounded-lg shadow-lg">
  <div class="text-6xl font-bold text-yellow-500 mb-2">270+</div>
  <div class="text-2xl">⭐ GitHub Stars</div>
</div>

<div class="p-8 bg-white rounded-lg shadow-lg">
  <div class="text-6xl font-bold text-blue-500 mb-2">13</div>
  <div class="text-2xl">🔱 Forks</div>
</div>

</div>

<div class="mt-12 space-y-4 text-lg max-w-2xl mx-auto">

<div class="p-4 bg-blue-50 rounded">
✅ **Type-Safe & Composable**: Engineered with TypeScript for reliability.
</div>

<div class="p-4 bg-green-50 rounded">
✅ **90% Test Coverage**: Built with Jest and Storybook, ensuring component robustness.
</div>

</div>

</div>

---

layout: two-cols
background: /backgrounds/blueprint-texture.png

---

<template v-slot:default>

# Bridging Mechanical Visualization and Digital Interaction

## 3D Product Configurator

<div class="space-y-4 text-lg">

**Real-time Rendering**: Built with Next.js and React Three Fiber.

**Performance Optimized**: Achieved a stable **60 FPS** average frame rate and reduced initial load times through efficient asset management.

**Modular Architecture**: Designed to bridge physical design principles with modern component-based UI.

</div>

<div class="mt-6 p-4 bg-orange-100 rounded-lg border-2 border-orange-400">
  <div class="text-3xl font-bold text-orange-600">⚡ 60 FPS</div>
  <div class="text-sm text-orange-800">Consistent Performance</div>
</div>

</template>

<template v-slot:right>

<div class="flex items-center justify-center h-full">
  <div class="text-center p-8 bg-gradient-to-br from-blue-50 to-blue-100 rounded-lg">
    <div class="text-6xl mb-4">🎮</div>
    <div class="text-2xl font-bold text-blue-900">Interactive 3D</div>
    <div class="text-lg text-blue-700">Product Configurator</div>
  </div>
</div>

</template>

---

layout: default
background: /backgrounds/grid-technical.png

---

# The Engineer's Toolkit

<div class="grid grid-cols-2 gap-8 px-8">

<div class="space-y-6">

<TechStack
  title="Frontend & Architecture"
  :items="[
    { name: 'React', icon: '⚛️' },
    { name: 'TypeScript', icon: '📘' },
    { name: 'Next.js', icon: '⚡' },
    { name: 'Tailwind CSS', icon: '🎨' },
    { name: 'Component-Based Architecture', icon: '🧩' }
  ]"
  color="#2563eb"
/>

<TechStack
  title="Cloud & DevOps"
  :items="[
    { name: 'AWS Certified Cloud Practitioner', icon: '☁️' },
    { name: 'GitHub Actions (CI/CD)', icon: '🔄' },
    { name: 'Docker', icon: '🐳' },
    { name: 'Serverless', icon: '⚡' }
  ]"
  color="#f59e0b"
/>

</div>

<div class="space-y-6">

<TechStack
  title="Backend & Databases"
  :items="[
    { name: 'Node.js', icon: '🟢' },
    { name: 'Express.js', icon: '🚂' },
    { name: 'PostgreSQL (PERN Stack)', icon: '🐘' },
    { name: 'REST/GraphQL APIs', icon: '🔌' },
    { name: 'Prisma', icon: '🔺' }
  ]"
  color="#16a34a"
/>

<TechStack
  title="Testing & QA"
  :items="[
    { name: 'Jest', icon: '🃏' },
    { name: 'Cypress', icon: '🌲' },
    { name: 'Playwright', icon: '🎭' },
    { name: 'Test-Driven Development (TDD)', icon: '✅' },
    { name: 'WCAG 2.1 Compliance', icon: '♿' }
  ]"
  color="#dc2626"
/>

</div>

</div>

---

layout: center
class: text-center
background: /backgrounds/grid-technical.png

---

# Applications in High-Stakes Environments

<div class="grid grid-cols-4 gap-6 mt-12 px-8">

<IndustryCard
  title="SaaS"
  icon="i-mdi-cloud-cog"
  description="Scalable multi-tenant architecture and 99.9% reliability."
  color="#2563eb"
/>

<IndustryCard
  title="HealthTech & Defense"
  icon="i-mdi-shield-plus"
  description="A deep-rooted understanding of compliance, security, and rigorous QA from direct industry experience."
  color="#dc2626"
/>

<IndustryCard
  title="FinTech"
  icon="i-mdi-bank"
  description="Focus on data integrity with PostgreSQL and a mindset geared towards transactional robustness."
  color="#f59e0b"
/>

<IndustryCard
  title="Industrial IoT"
  icon="i-mdi-cog-sync"
  description="Unique ability to bridge physical systems and digital infrastructure."
  color="#16a34a"
/>

</div>

---

layout: default
background: /backgrounds/grid-technical.png

---

# Moving from Reactive Fixes to Proactive Design

<ComparisonSlide
  leftTitle="What Is: The Cost of Unengineered Code"
  rightTitle="What Could Be: The Value of Engineered Systems"
  :leftItems="[
    'Brittle features that break under load',
    'Escalating technical debt',
    'Slow, risky deployments'
  ]"
  :rightItems="[
    'Robust, scalable architecture',
    'Long-term maintainability',
    'Accelerated, reliable development cycles'
  ]"
  leftColor="#dc2626"
  rightColor="#16a34a"
/>

---

layout: cover
background: /backgrounds/bridge-sunset.png
class: text-center

---

<div class="text-white drop-shadow-lg">

# Let's build software that's not just functional for today, but engineered for the decade ahead.

</div>

---

layout: center
class: text-center
background: /backgrounds/grid-technical.png

---

# Architect the Solution.

<div class="mt-12 max-w-2xl mx-auto">

<div class="mb-8">
  <div class="text-4xl font-bold text-blue-900">Timothy DeHof</div>
  <div class="text-2xl text-blue-700 mt-2">Full-Stack Engineer</div>
</div>

<div class="grid grid-cols-2 gap-4 text-lg mb-8">
  <div class="p-3 bg-white rounded shadow">
    📧 ttdehof@gmail.com
  </div>
  <div class="p-3 bg-white rounded shadow">
    📱 (904) 704-1790
  </div>
  <div class="p-3 bg-white rounded shadow col-span-2">
    🔗 <a href="https://linkedin.com/in/tim-dehof" class="text-blue-600 hover:underline">linkedin.com/in/tim-dehof</a>
  </div>
  <div class="p-3 bg-white rounded shadow col-span-2">
    💻 <a href="https://github.com/timDeHof" class="text-blue-600 hover:underline">github.com/timDeHof</a>
  </div>
</div>

<div class="mt-8">
  <a href="#" class="inline-block px-12 py-4 bg-blue-600 text-white rounded-lg text-xl font-semibold hover:bg-blue-700 transition-colors shadow-lg">
    Schedule a technical deep-dive
  </a>
</div>

</div>
