<template>
  <div>
    <h2>TESTE SLOT-SCOPE $SLOTS</h2>

    <slot
      v-for="(cell, index) in row"
      :name="'cell-' + index"
      :cell="cell"
      :index="index">

      <tr :key="index">
        <td :key="index">{{ cell }}</td>
      </tr>
    </slot>
  </div>
</template>

<script>
  export default {
    props: {
      row: Array
    }
  }
</script>

