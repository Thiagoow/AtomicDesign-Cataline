<template>
  <Container class="home">
    <Header class="header" />
    <Presentation class="presentation" />
    <Skills class="skills" />
  </Container>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { Container } from "@/components/bosons";
import { Header, Presentation, Skills } from "@/components/organisms";

export default defineComponent({
  components: { Container, Header, Presentation, Skills },
});
</script>

<style lang="scss" scoped>
.home {
  margin: 0.8rem auto;
  display: grid;
  grid-gap: 5rem;
}
.presentation {
  margin-top: -5rem;
}
.skills {
  margin-top: -5rem;
}
</style>
