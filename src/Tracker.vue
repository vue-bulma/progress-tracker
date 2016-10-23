<template>
  <ul :class="{
    'progress-tracker': true,
    [`progress-tracker--${alignment}`]: alignment,
    'progress-tracker--border': border,
    'progress-tracker--spaced': spaced,
    'progress-tracker--word': word,
    [`progress-tracker--word-${textAlign}`]: wordAlign,
    'progress-tracker--text': text
  }">
    <slot></slot>
  </ul>
</template>

<script>
export default {
  props: {
    alignment: String,
    step: Number,
    border: Boolean,
    spaced: Boolean,
    word: Boolean,
    wordAlign: String,
    text: Boolean,
    textAlign: String
  },

  computed: {
    $stepItems () {
      return this.$children.filter(child => child._isStepItem)
    }
  }
}
</script>

<style lang="scss">
@import '~bulma/sass/utilities/variables';
@import "~progress-tracker/app/styles/_progress-tracker.scss";

.progress-step:not(:last-child)::after {
  z-index: 0;
}
</style>
