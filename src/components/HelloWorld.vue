<script setup lang="ts">
import { ref } from "vue";

defineProps({ msg: String });
const count = ref(0);
</script>

<template>
  <h1 class="font-pacifico">{{ msg }}</h1>

  <div class="card">
    <button type="button" class="btn ma block" @click="count++">
      count is {{ count }}
    </button>
    <p class="flex">
      <i class="color-emerald i-ion-information-circle-sharp"></i>
      Edit
      <code>components/HelloWorld.vue</code>
      to test HMR
    </p>
  </div>

  <p>
    Check out
    <a href="https://vuejs.org/guide/quick-start.html#local" target="_blank"
      >create-vue</a
    >, the official Vue + Vite starter
  </p>

  <p>
    Install<a href="https://github.com/johnsoncodehk/volar" target="_blank"
      >Volar</a
    >in your IDE for a better DX
  </p>

  <p class="color-gray">Click on the Vite and Vue logos to learn more</p>

  <h2><code>sanitize/forms</code> example</h2>

  <form class="flex flex-col gap-4 mb-10">
    <input type="text" />
    <input type="search" />
    <input type="email" />
    <input type="number" />
    <label>
      <input type="checkbox" />
      checkbox
    </label>
    <label>
      <input type="radio" name="radio" />
      Radio
    </label>
    <label>
      <input type="radio" name="radio" />
      Radio
    </label>
    <textarea cols="30" rows="10"></textarea>
    <select>
      <option value="1">option 1</option>
      <option value="2">option 2</option>
      <option value="3">option 3</option>
      <option value="4">option 4</option>
      <option value="5">option 5</option>
    </select>
    <input type="color" />
    <input type="date" />
    <button>Submit</button>
  </form>
</template>
