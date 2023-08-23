<template>
<div class="sudoku-quadrant" >
  <Field v-for="n in 9" :key="n" />
</div>
</template>

<script>
import Field from './Field.vue'

export default {
  name: 'Sudoku-Quadrant',
  components: {
    Field,
  },
}
</script>

<style>
.sudoku-quadrant {
  display: flex;
  flex-flow: row wrap;
}
</style>
