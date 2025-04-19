---
title: v-animate
navigation: true
header: true
main:
  fluid: false
---
# v-animate

::alert{type="warning"}
🚧 We are currently working on further improvements and adding more functionality to the directive. <br />Please be aware that this particular aspect may undergo frequent changes. 🚧
::


``v-animate`` is the best chooise for the ultra simple Animation like hover or click eventbase Animation.  <br/>
add `v-animate` to a Element and give it some `AnimationParams` directily. Done.
In this case you **dont** get back a ``ref`` of `JSAnimation`. 
<br />
<br />
For more detailed information regarding the animation object, please refer to the [Anime.js V4 Documatation](https://animejs.com/documentation/animation).

```vue
<template>
  <div>
    <div v-animate="{ x: 100 }" class="box" />
  </div>
</template>
```

You can also choose to extract the ``AnimationParams`` into a separate ``ref``, either as a complete object or for specific values.
This allows you to manage your basic animation logic within the setup, as demonstrated in the following example:


```vue
<template>
  <div>
    <div v-animate="{ x: xVal }" class="box" />
    <pre>xVal: {{ xVal }}</pre>
  </div>
</template>

<script lang="ts" setup>
const xVal = ref(30);
</script>
```