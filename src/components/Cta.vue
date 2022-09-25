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
  background-color: $dt-c-black;
  color: $dt-c-white;
  border-radius: 4px;
  &--default {
    color: $dt-c-white; // Placeholder
  }
  &--landing {
    border: 2px solid $dt-c-secondary-accent;
  }
}
</style>
