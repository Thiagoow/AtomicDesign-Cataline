<template>
  <div class="skills">
    <Skill
      title="Front-End"
      text="Lorem ipsum dolor sit amet consectetur adipisicing elit. Amet aperiam culpa dolor officia quis similique dolorem optio tempora earum sequi mollitia ex iure consequatur incidunt aut, ratione, animi velit necessitatibus."
    />
    <Skill
      title="UX/UI"
      text="Lorem ipsum dolor sit amet consectetur adipisicing elit. Amet aperiam culpa dolor officia quis similique dolorem optio tempora earum sequi mollitia ex iure consequatur incidunt aut, ratione, animi velit necessitatibus."
    />
    <Skill
      title="Back-End"
      text="Lorem ipsum dolor sit amet consectetur adipisicing elit. Amet aperiam culpa dolor officia quis similique dolorem optio tempora earum sequi mollitia ex iure consequatur incidunt aut, ratione, animi velit necessitatibus."
    />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { Skill } from "@/components/molecules";

export default defineComponent({
  components: { Skill },
});
</script>

<style lang="scss" scoped>
.skills {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 5rem;
}
</style>
