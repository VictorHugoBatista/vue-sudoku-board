<template>
<div class="sudoku-board">
  <Quadrant v-for="n in 9"
    :quadrantClass="`sudoku-quadrant-${n}`"
    :key="n" />
</div>
</template>

<script>
import Quadrant from './Quadrant.vue'

export default {
  name: 'Sudoku-Board',
  components: {
    Quadrant,
  },
}
</script>

<style>
.sudoku-board {
  display: flex;
  height: 900px;
  flex-flow: row wrap;
  justify-content: center;
  margin: 20px 0;
  width: 900px;
}
</style>
