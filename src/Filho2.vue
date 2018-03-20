<template>
  <div>
    <h2>TESTE SLOT-SCOPE FILHO-2</h2>

    <slot name="list-items" v-for="item in items" :text="item.text"></slot>
  </div>
</template>

<script>
export default {
  data () {
    return {
      items: [
        { text: 'texto 1' },
        { text: 'texto 2' },
        { text: 'texto 3' }
      ]
    }
  }
}
</script>
