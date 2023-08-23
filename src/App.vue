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
  background-color: #dceef5;
  border-radius: 7px;
  display: flex;
  height: 100%;
  justify-content: center;
  width: 100%;
}
</style>
