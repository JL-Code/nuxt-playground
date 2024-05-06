<script lang="ts" setup>
const links = useBreadcrumbItems(); // uses the current route
</script>
<template>
  <div>{{ links }}</div>
</template>
