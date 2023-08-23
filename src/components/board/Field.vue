<template>
<div class="sudoku-field-container">
  <input class="sudoku-field" type="text" value="1" />
</div>
</template>

<script>
export default {
  name: 'Sudoku-Field',
}
</script>

<style>
.sudoku-field {
  background-color: transparent;
  border: none;
  border-radius: 3px;
  font-size: 15px;
  margin: 10px;
  text-align: center;
  height: calc(100% - 20px);
  transition: 250ms ease-in;
  width: calc(100% - 20px);
}

.sudoku-field:focus {
  background-color: rgba(255, 255, 255, .6);
  box-shadow: 2px 2px 5px -2px rgba(0, 0, 0, .4);
  outline: none;
}
</style>
