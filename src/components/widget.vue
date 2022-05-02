<script setup lang="ts">
import { PhChatTeardropDots } from "phosphor-vue";
import { Popover, PopoverButton, PopoverPanel } from "@headlessui/vue";
</script>

<template>
  <Popover class="container">
    <PopoverPanel>Abriu</PopoverPanel>
    <PopoverButton class="button group">
      <PhChatTeardropDots weight="bold" class="icon" />

      <div
        class="feedback-container group-hover:max-w-xs transition-all duration-500 ease-linear"
      >
        <span class="feedback-text">Feedback</span>
      </div>
    </PopoverButton>
  </Popover>
</template>

<style scoped>
.container {
  @apply absolute bottom-5 right-5 w-fit;
}
.button {
  @apply flex h-12 px-3 bg-brand-500 rounded-full items-center;
}

.icon {
  @apply h-6 w-6 text-white;
}

.feedback-container {
  @apply max-w-0 overflow-hidden;
}

.feedback-text {
  @apply text-white pl-2;
}
</style>
