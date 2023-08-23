<template>
<div>
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
