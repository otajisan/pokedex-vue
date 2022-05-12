<template>
  <div class="search">
    <h1>{{ name }}</h1>
  </div>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "DisplayPokedex",
  props: {
    name: String,
  },
});
</script>
