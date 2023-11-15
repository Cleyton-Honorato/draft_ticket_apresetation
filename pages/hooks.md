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
      Hooks
      <mdi:react/>
    </span>
  </div>

```js
import { useState, useEffect } from "react";

const useFetch = (url) => {
  const [data, setData] = useState(null);

  useEffect(() => {
    fetch(url)
      .then((res) => res.json())
      .then((data) => setData(data));
  }, [url]);

  return [data];
};

export default useFetch;
```
</div>

<div class="mt-10 ml-30">
  <div>
    <span class="text-xl text-black text-opacity-60" style="font-weight:600;">
      Composable
      <logos:vue/>
    </span>
  </div>

```js
// useFetch.ts
import { ref } from 'vue'

export function useFetch(url) {
  const data = ref(null)
  const error = ref(null)

  fetch(url)
    .then((res) => res.json())
    .then((json) => (data.value = json))
    .catch((err) => (error.value = err))

  return { data, error }
}
// component
<script setup>
import { useFetch } from './fetch.js'

const { data, error } = useFetch('...')
</script>
```
</div>


