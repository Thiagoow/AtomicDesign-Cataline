<template>
  <!--Criamos nossa molécula de pesquisa direto,
    sem antes criar os átomos, pois ela não é reutilizada
    em nenhum lugar do nosso website. Tornando desnecessário
    então, dividi-la em átomos, ainda mais por ser apenas uma
    barrinha de pesquisa com um ícone 😁-->
  <form class="pesquisa">
    <input type="search" placeholder="Buscar" />
    <button type="submit">
      <img src="@/assets/images/icons/search.svg" alt="search" />
    </button>
  </form>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({})
</script>

<style lang="scss" scoped>
.pesquisa {
  position: relative;
  width: max-content;
  input {
    border: none;
    border-radius: 1rem;
    padding: 0.5rem 1rem;
    box-shadow: 0px 5px 5px rgba(#000000, 0.08);
    &::placeholder {
      color: #a9b0be;
    }
  }
  button {
    position: absolute;
    right: 3px;
    top: 50%;
    transform: translateY(-50%);
    width: 30px;
    height: 30px;
    background: #ff895f;
    border: none;
    border-radius: 5rem;
    display: grid;
    justify-items: center;
    align-items: center;
  }
}
</style>
