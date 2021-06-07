<template>
  <div class="app">
    <Home />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { Home } from "@/components/templates";

export default defineComponent({
  components: { Home },
});
</script>

<style lang="scss" scoped></style>
