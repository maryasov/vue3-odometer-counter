# vue3-odometer-counter

> Vue.js(v3.2+) component wrap for Odometer.js

> Forked from [vangleer/vue3-odometer](https://github.com/vangleer/vue3-odometer)
 
## Installation

``` bash
npm install --save odometer-counter vue3-odometer-counter
```

## Usage
``` vue
<template>
  <Vue3Odometer class="o-text" :value="number" />
  <button @click="update">update number</button>
</template>

<script lang="ts" setup>
import { ref } from 'vue'
import Vue3Odometer from 'vue3-odometer-counter'
import 'odometer-counter/themes/odometer-theme-main.css'
const number = ref(100)

function update() {
  number.value = Math.floor(Math.random() * 1000)
}
</script>

<style>
.o-text {
  color: red;
}
</style>
```

## Properties

* `value` **[Number]**

  Optional; `0` by default.

* `format` **[String]**

  Optional;

* `theme` **[String]**

  Optional; `default` by default.

* `duration` **[Number]**

  Optional;

* `animation` **[String]**

  Optional;

* `formatFunction` **[Function]**

  Optional;

See more [Odometer.js](http://github.hubspot.com/odometer/)

## Methods

* `renderInside`
* `watchForMutations`
* `startWatchingMutations`
* `stopWatchingMutations`
* `cleanValue`
* `bindTransitionEnd`
* `resetFormat`
* `renderDigit`
* `formatDigits`
* `insertDigit`
* `addDigit`
* `addSpacer`
* `animate`
* `animateCount`
* `getDigitCount`
* `getFractionalDigitCount`
* `resetDigits`
* `animateSlide`
* `render`
* `update`

Learn more [Odometer.js](http://github.hubspot.com/odometer/)


# License

MIT
