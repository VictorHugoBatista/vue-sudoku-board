<template>
<div class="sudoku-board">
  <Grid
    gridItemBorderColor="#9c1a77"
    gridItemBorderStyle="solid"
  >
    <Quadrant />
  </Grid>
</div>
</template>

<script>
import Grid from '../layout/Grid.vue'
import Quadrant from './Quadrant.vue'

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
  height: 600px;
  justify-content: center;
  margin: 20px 0;
  width: 600px;
}
</style>
