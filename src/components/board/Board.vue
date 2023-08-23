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
  background-color: #dceef5;
  border-radius: 7px;
  box-shadow: inset 0px 0px 10px -4px rgba(0,0,0,0.6);
  display: flex;
  height: 600px;
  justify-content: center;
  padding: 20px;
  width: 600px;
}
</style>
