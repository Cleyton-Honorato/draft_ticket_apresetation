---
class: flex flex-1 flex-row bg-gradient-to-r from-#b19fe3 to-#4c12a1
transition: slide-left
highlighter: shiki
---

<!-- LOGO -->
<div class="w-50 h-20 absolute top-0 left-0">
  <img src="/assets/tr-logo@2x.png" class="w-30" />
</div>

<div class="mt-20">
  <div>
    <span class="text-xl text-black text-opacity-60" style="font-weight:600;">
      JSX
      <mdi:react/>
    </span>
  </div>

  ```js
  export default function Component() {
    return (
      <div>
        <h1>Hello Word</h1>
      </div>
    );
  }
  ```
</div>

<div class="mt-20 ml-50">
  <div>
    <span class="text-xl text-black text-opacity-60" style="font-weight:600;">
      SFC
      <logos:vue/>
    </span>
  </div>

```js{all|1,2,3,4|6,7,8|10,11,12,13,14,15}
<script setup>
  import { ref } from 'vue'
  const greeting = ref('Hello World!')
</script>

<template>
  <p class="greeting">{{ greeting }}</p>
</template>

<style>
  .greeting {
    color: red;
    font-weight: bold;
  }
</style>
```
</div>

