<template>
  <li class="progress-step" :class="{ 'is-active': isActived, 'is-complete': isCompleted }">
    <span class="progress-marker"></span>
    <span class="progress-text">
      <h4 class="progress-title"></h4>
    </span>
  </li>
</template>

<script>
export default {
  props: {
    isActived: Boolean,
    isCompleted: Boolean
  }
}
</script>
