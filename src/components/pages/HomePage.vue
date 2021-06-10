<template>
  <HomeTemplate />
  <!--Como nosso website é estático, ou seja:
  não recebe nenhum tipo de chamada na API, OU, nesse caso:
  não possui nenhum tipo de back-end:
  
  Poderíamos ter abolido o uso das pages. E usado apenas o
  HomeTemplate como componente principal.
  MAS, DO CONTRÁRIO, precisaríamos sim, da pasta e componentes pages,
  para realizar todas as chamadas na API, e conexão com dB.
  
  OU SEJA = Apenas as páginas fazem o server side rendering. 
  (renderização de servirdor/carregamento do back-end)
  
  ALÉM DISSO, no Nuxt.js, não precisamos fazer TODA HORA, a exportação
  e importação dos componentes. Então no mínimo 1/3 do trabalho é 😎😉
  cortado, e não perdemos tempo com esse negócio chato.-->
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { HomeTemplate } from "@/components/templates";

export default defineComponent({
  components: { HomeTemplate },
  /*Todos os componentes da página, teriam acesso aos dados 
  injetados no Vuex, aqui com o tag template.*/
  created() {
    //Chamada/requisição na API
  }
});
</script>
