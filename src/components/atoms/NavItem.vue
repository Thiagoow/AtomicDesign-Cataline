<template>
  <a class="navItem" :href="link">
    {{ text }}
  </a>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  props: {
    text: {
      type: String,
      required: true
    },
    link: {
      type: String,
      required: true
    }
  }
});
</script>

<style lang="scss" scoped>
.navItem {
  color: #293947;
  text-decoration: none;
  font-size: 1.3rem;
}
</style>
