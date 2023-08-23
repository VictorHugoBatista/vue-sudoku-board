<template>
<div class="sudoku-board">
  <Quadrant v-for="n in 9" :key="n" />
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
  align-items: center;
  display: flex;
  height: 900px;
  flex-flow: row wrap;
  justify-content: center;
  width: 900px;
}
</style>
