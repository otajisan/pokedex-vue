<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/img/morningcode.png" />
    <form>
      <input id="search" v-model.lazy="pokemonName" />
    </form>
    <p>{{ pokemonName }}</p>
    <DisplayPokedex name="test" />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import DisplayPokedex from "@/components/DisplayPokedex.vue"; // @ is an alias to /src

export default defineComponent({
  name: "HomeView",
  components: {
    DisplayPokedex,
  },
});
</script>
