<template>
  <ClientOnly>
    <iframe
      :src="src"
      class="rounded-lg relative h-96 w-full"
    />
  </ClientOnly>
</template>

<script setup lang="ts">
const appConfig = useAppConfig()

const src = computed(() => {
  return `https://ui.nuxt.com/examples/content-search-example?primary=${appConfig.ui.colors.primary}&neutral=${appConfig.ui.colors.neutral}`
})
</script>
