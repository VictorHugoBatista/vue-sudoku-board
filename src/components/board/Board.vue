<template>
<div>
  <Quadrant v-for="n in 9" :key="n" />
</div>
</template>

<script>
import Quadrant from './Quadrant.vue'

export default {
  name: 'Sudoku-Board',
  components: {
    Quadrant,
  }
}
</script>
