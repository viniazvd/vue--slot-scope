<template>
  <div>
    <h2>TESTE SLOT-SCOPE FILHO-1</h2>

    <slot name="cabecalho">conteudo default do slot cabecalho</slot>
    <slot text="conteúdo do slot default aqui"></slot>
    <slot name="conteudo" text="conteudo default do slot conteudo"></slot>
    <slot name="footer">conteudo default do slot footer</slot>
  </div>
</template>

