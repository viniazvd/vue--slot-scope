<template>
  <div id="app">
    <filho1>
      <div slot-scope="propsSlotDefault">
        {{ propsSlotDefault.text }}
      </div>

      <!-- <div slot="conteudo" slot-scope="props"> -->
      <!--   {{ props.text }} -->
      <!-- </div> -->

      <!-- o bloco comentado abaixo tem o mesmo efeito que o de cima -->
      <!-- mas com o uso da técnica de desestruturação -->

      <div slot="conteudo" slot-scope="{ text }">
        {{ text }}
      </div>
    </filho1>

    <filho2>
      <li slot="list-items" slot-scope="props">
        {{ props.text }}
      </li>
    </filho2>
  </div>
</template>

<script>
import filho1 from './Filho1.vue';
import filho2 from './Filho2.vue';

export default {
  components: { filho1, filho2 }
}
</script>

<style scoped>
#app {
  display: flex;
  align-items: center;
  flex-direction: column;
}
</style>

