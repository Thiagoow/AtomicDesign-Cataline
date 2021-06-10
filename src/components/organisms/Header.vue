<template>
  <div class="header"><Logo /> <NavBar /> <Pesquisa /></div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { Logo } from "@/components/atoms";
import { NavBar, Pesquisa } from "@/components/molecules";

export default defineComponent({
  components: { Logo, NavBar, Pesquisa }
});
</script>

<style lang="scss" scoped>
.header {
  width: 100%;
  display: grid;
  //1 coluna + 2 colunas com o tamanho auto:
  grid-template-columns: 160px repeat(2, auto);
  align-items: center;
  justify-content: space-between;
}
</style>
