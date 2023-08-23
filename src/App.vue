<template>
  <div id="app" class="sudoku-container">
    <Board />
  </div>
</template>

<script>
import Board from './components/board/Board.vue'

export default {
  name: 'App',
  components: {
    Board,
  }
}
</script>

<style>
.sudoku-container {
  align-items: center;
  background-color: #fafafe;
  display: flex;
  height: 100vh;
  justify-content: center;
  width: 100%;
}
</style>
