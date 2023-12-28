<script setup lang="ts">
import { useCounter } from '@vueuse/core'

const { count, inc, dec } = useCounter()
</script>

<template>
  <div>
    <h1 class="text-xl">useCounter</h1>
    <p class="mt-4">Counter: {{ count }}</p>
    <div class="flex gap-2 mt-4">
      <button
        type="button"
        @click="inc()"
        class="rounded grid place-content-center bg-gray-200 min-w-10 min-h-10 p-2 cursor-pointer"
      >
        +
      </button>
      <button
        type="button"
        @click="dec()"
        class="rounded grid place-content-center bg-gray-200 min-w-10 min-h-10 p-2 cursor-pointer"
      >
        -
      </button>
    </div>
  </div>
</template>
