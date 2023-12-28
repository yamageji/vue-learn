<script setup lang="ts">
import { useCounter } from '@vueuse/core'
import BaseLink from '@/components/BaseLink.vue'

const { count, inc, dec } = useCounter()
</script>

<template>
  <div>
    <h1 class="text-xl">useCounter</h1>
    <p class="mt-4">
      参照：<BaseLink to="https://vueuse.org/shared/useCounter/#usecounter">useCounter</BaseLink>
    </p>
    <p class="mt-4">Counter: {{ count }}</p>
    <div class="flex mt-4 gap-2">
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
