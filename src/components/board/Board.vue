<template>
<div class="sudoku-board">
  <Grid
    gridItemBorderColor="#946988"
    gridItemBorderStyle="solid"
  >
    <Quadrant />
  </Grid>
</div>
</template>

<script>
import Quadrant from './Quadrant.vue'
import Grid from '../layout/Grid.vue'

export default {
  name: 'Sudoku-Board',
  components: {
    Grid,
    Quadrant,
  },
}
</script>

<style>
.sudoku-board {
  display: flex;
  height: 900px;
  justify-content: center;
  margin: 20px 0;
  width: 900px;
}
</style>
