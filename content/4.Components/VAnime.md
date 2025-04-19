---
title: VAnime
navigation: true
header: true
main:
  fluid: false
---
# VAnime

::alert{type="warning"}
🚧 We are currently working on further improvements and adding more functionality to the Components. <br />
At the Moment the Components are not ready yet. Please be aware that this particular aspect may undergo frequent changes. 🚧
::



For more complex and advanced animations, the ``<VAnime />`` component offers the best approach.
This component provides all the necessary functionality of the Animation object in a simple and `` Vue-style`` manner.
You can customize it with various props and also utilize the available events/emits.

Under the Hood the Component handle all your `AnimationParams` to give you the best DX.

```vue
<template>
  <div>
    <VAnimate
      is="div"
      :animate="{
        x: 300,
        rotate: 120,
      }"
      class="box"
    />
  </div>
</template>
```