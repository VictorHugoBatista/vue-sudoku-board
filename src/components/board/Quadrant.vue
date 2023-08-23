<template>
<div class="sudoku-quadrant" :class="quadrantClass" >
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
  props: [
    'quadrantClass',
  ],
}
</script>

<style>
.sudoku-quadrant {
  display: flex;
  flex: 0 1 30%;
  flex-flow: row wrap;
}

.sudoku-quadrant-1 {
  border: 3px solid black;
  border-width: 0 2px 2px 0;
}
.sudoku-quadrant-2 {
  border: 3px solid black;
  border-width: 0 2px 2px 2px;
}
.sudoku-quadrant-3 {
  border: 3px solid black;
  border-width: 0 0 2px 2px;
}
.sudoku-quadrant-4 {
  border: 3px solid black;
  border-width: 2px 2px 2px 0;
}
.sudoku-quadrant-5 {
  border: 3px solid black;
  border-width: 2px;
}
.sudoku-quadrant-6 {
  border: 3px solid black;
  border-width: 2px 0 2px 2px;
}
.sudoku-quadrant-7 {
  border: 3px solid black;
  border-width: 2px 2px 0 0;
}
.sudoku-quadrant-8 {
  border: 3px solid black;
  border-width: 2px 2px 0 2px;
}
.sudoku-quadrant-9 {
  border: 3px solid black;
  border-width: 2px 0 0 2px;
}
</style>
