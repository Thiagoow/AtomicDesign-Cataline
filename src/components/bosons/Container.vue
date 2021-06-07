<template>
  <div class="container">
    <!--Todo o layout do website Marcos, fica dentro de um container,
    o qual dá um espaçamento de margem esquerda e direita para o website, 
    centralizando o contéudo. Sendo assim, para não criarmos do zero esse 
    container, criamos ele como um bóson.-->
    <slot />
    <!--Criando essa div vazia slot, apenas para conseguirmos
    exportar nosso componente.-->
  </div>
</template>

<style lang="scss" scoped>
/*Criando o espaçamento:*/
.container {
  width: 85%;
  max-width: 1150px;
  /*Margem de zero em cima e embaixo, 
  e automático, na direita e esquerda:*/
  margin: 0 auto;
}
</style>
