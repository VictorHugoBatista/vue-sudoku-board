<template>
<div class="sudoku-quadrant" >
  <Grid
    gridItemBorderColor="#a5b879"
    gridItemBorderStyle="dotted"
  >
    <Field />
  </Grid>
</div>
</template>

<script>
import Grid from '../layout/Grid.vue'
import Field from './Field.vue'

export default {
  name: 'Sudoku-Quadrant',
  components: {
    Field,
    Grid,
  },
}
</script>

<style>
.sudoku-quadrant {
  display: flex;
  flex-flow: row wrap;
}
</style>
