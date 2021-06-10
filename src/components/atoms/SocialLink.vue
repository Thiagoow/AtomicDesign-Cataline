<template>
  <a class="socialLink" :href="link" target="_blank">
    <!--O target "_blank" permite que o link seja aberto em outra
    aba do browser, sem fechar assim, o website.-->
    <img :src="iconPath" :alt="name" />
  </a>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  props: {
    name: { type: String, required: true },
    link: { type: String, required: true },
    icon: { type: String, required: true }
  },
  computed: {
    //Para definir o caminho dos ícones e não se repetir sempre:
    iconPath(): string {
      return require(`@/assets/images/icons/${this.icon}`);
    }
  }
});
</script>

<style lang="scss" scoped>
.socialLink {
  background-color: #ff895f;
  width: 47px;
  height: 47px;
  border-radius: 5rem;
  display: grid;
  justify-items: center;
  align-items: center;
  transition: transform 0.2s linear;
  &:hover {
    transform: scale(1.1);
  }
  img {
    width: 23px;
    height: 23px;
  }
}
</style>
