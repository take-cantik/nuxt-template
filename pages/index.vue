<template>
  <div>
    <h1>{{ hello }}</h1>
    <Tutorial />
  </div>
</template>

<script lang="ts">
import { defineComponent, ref } from "@nuxtjs/composition-api";

export default defineComponent({
  setup() {
    const hello = ref<string>("Hello, world!");

    return {
      hello,
    };
  },
});
</script>
