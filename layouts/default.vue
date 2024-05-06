<script setup>
const items = useBreadcrumbItems(); // uses the current route
</script>
<template>
  <div>
    <nav aria-label="Breadcrumbs">
      <ul>
        <li v-for="(item, key) in items" :key="key">
          <NuxtLink v-bind="item">
            {{ item.label }}
          </NuxtLink>
        </li>
      </ul>
    </nav>
    <slot />
  </div>
</template>
