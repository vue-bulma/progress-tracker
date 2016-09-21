# ProgressTracker

ProgressTracker component is based on [progress-tracker](http://nigelotoole.github.io/progress-tracker/) for Vue Bulma.


## Installation

```
$ npm install vue-bulma-progress-tracker --save
```


## Examples

```vue
<template>
  <progress-tracker>
    <step-item v-for="n in [1, 2, 3, 4, 5]" :is-complete="n < 3" :is-active="n === 3"></step-item>
  </progress-tracker>
</template>

<script>
import ProgressTracker, { StepItem } from 'vue-bulma-progress-tracker'

export default {
  components: {
    ProgressTracker,
    StepItem
  }
}
</script>
```


## Badges

![](https://img.shields.io/badge/license-MIT-blue.svg)
![](https://img.shields.io/badge/status-stable-green.svg)

---

> [fundon.me](https://fundon.me) &nbsp;&middot;&nbsp;
> GitHub [@fundon](https://github.com/fundon) &nbsp;&middot;&nbsp;
> Twitter [@_fundon](https://twitter.com/_fundon)

