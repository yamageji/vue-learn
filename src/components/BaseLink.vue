<script setup lang="ts">
type Props = {
  to: string
}
defineProps<Props>()
</script>

<template>
  <a :href="to" class="text-blue-500 hover:underline underline-offset-1">
    <slot></slot>
  </a>
</template>
