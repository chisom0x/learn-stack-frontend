<template>
  <div class="flex p-8 justify-center">
    <input
      type="text"
      class="rounded border-2 border-grey-200 w-full"
      placeholder="search for meals"
    />
  </div>
</template>

<script setup>
import { computed } from "vue";
import store from "../store";

const meals = computed(() => store.state.meals);
</script>
