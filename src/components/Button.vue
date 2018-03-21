<template>
  <button :class="classes">
    <span>{{ icon }}</span>

    <span v-if="!!$slots.default" class="text">
      <slot />
    </span>
  </button>
</template>

<script>
export default {
  props: {
    icon: String,
  },
  computed: {
    classes () {
      return ['Button', { '-empty': !!this.$slots.default }]
    }
  }
}
</script>

