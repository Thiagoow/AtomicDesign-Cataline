<template>
  <div class="socialNetworks">
    <SocialLink name="GitHub" link="#" icon="github.svg" />
    <SocialLink name="Facebook" link="#" icon="facebook.svg" />
    <SocialLink name="Twitter" link="#" icon="twitter.svg" />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { SocialLink } from "@/components/atoms";

export default defineComponent({
  components: { SocialLink }
});
</script>

<style lang="scss" scoped>
.socialNetworks {
  display: grid;
  grid-gap: 1rem;
}
</style>
