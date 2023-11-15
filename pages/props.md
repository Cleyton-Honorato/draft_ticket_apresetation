---
class: flex bg-gradient-to-r from-#b19fe3 to-#4c12a1
transition: slide-left
---

<!-- LOGO -->
<div class="w-50 h-20 absolute top-0 left-0">
  <img src="/assets/tr-logo@2x.png" class="w-30" />
</div>

<div class="mt-20">
  <div>
    <span class="text-xl text-black text-opacity-60" style="font-weight:600;">
      props
      <mdi:react/>
    </span>
  </div>

```js
function Avatar({ person, size }) {
  // person and size are available here
}

export default function Profile() {
  return (
    <Avatar
      person={{ name: "Lin Lanying", imageId: "1bX5QH6" }}
      size={100}
    />
  );
}
```
</div>

<div class="mt-10 ml-10">
  <div>
    <span class="text-xl text-black text-opacity-60" style="font-weight:600;">
      props
      <logos:vue/>
    </span>
  </div>

```js {all|12|7}
// Importing the ./Avatar.vue
<script setup>
  import Avatar from '@/components/Avatar.vue';
</script>

<tamplate>
  <Avatar :src="path" />
</template>

// Avatar component ./Avatar.vue
<script setup>
  const props = defineProps({ src: string; })
</script>

<template>
  <div>
    <img src={{src}} />
  </div>
</template>
```
</div>


