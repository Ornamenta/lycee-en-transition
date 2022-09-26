<script setup>
defineProps({
  type: {
    type: String,
    required: false,
    default: "default",
  },
  btn_text: {
    type: String,
    required: true,
  },
});
</script>

<template>
  <button :class="`cta cta--${type}`">{{ btn_text }}</button>
</template>

<style scoped lang="scss">
.cta {
  height: var(--dt-s-cta-height);
  padding: 0 25px;
  font-size: 1.4rem;
  background-color: var(--dt-c-background);
  font-family: var(--dt-f-cta-text);
  color: var(--dt-c-on-background);
  border-radius: calc(var(--dt-s-cta-height) / 2);
  &--default {
    color: var(--dt-c-on-background); // Placeholder
  }
  &--landing {
    border: 2px solid var(--dt-c-secondary);
  }
}
</style>
