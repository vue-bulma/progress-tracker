<template>
  <ul class="progress-tracker">
    <slot></slot>
  </ul>
</template>

<script>
export default {
  props: {
    step: Number
  },

  computed: {
    $stepItems () {
      return this.$children.filter(child => child._isStepItem)
    }
  }
}
</script>

<style lang="scss">
@import "~progress-tracker/app/styles/progress-tracker";
</style>
