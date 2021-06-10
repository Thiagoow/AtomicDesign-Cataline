<template>
  <nav class="navBar">
    <NavItem text="Home" link="/Home" />
    <NavItem text="Quem sou eu?" link="/Sobre" />
    <NavItem text="Habilidades" link="/Habilidades" />
    <NavItem text="Contato" link="/Contato" />
  </nav>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { NavItem } from '@/components/atoms'

export default defineComponent({
  components: { NavItem }
})
</script>

<style lang="scss" scoped>
.navBar {
  width: max-content;
  display: grid;
  grid-auto-flow: column;
  grid-gap: 2.5rem;
}
</style>
