<template>
<div class="grid" >
  <div v-for="n in 9" :key="n"
    class="grid-item" :class="`grid-item-${n}`"
    :style="{borderColor: gridItemBorderColor, borderStyle: gridItemBorderStyle}">
    <slot></slot>
  </div>
</div>
</template>

<script>
export default {
  name: 'Sudoku-Grid',
  props: [
    'gridItemBorderColor',
    'gridItemBorderStyle',
  ],
}
</script>

<style>
.grid {
  align-items: stretch;
  display: flex;
  flex-flow: row wrap;
}

.grid-item {
  display: flex;
  flex: 1 1 calc(33.3333% - 4px);
  flex-flow: row wrap;
  justify-content: center;
}

.grid-item-1 {
  border-width: 0 2px 2px 0;
}

.grid-item-2 {
  border-width: 0 2px 2px 2px;
}

.grid-item-3 {
  border-width: 0 0 2px 2px;
}

.grid-item-4 {
  border-width: 2px 2px 2px 0;
}

.grid-item-5 {
  border-width: 2px;
}

.grid-item-6 {
  border-width: 2px 0 2px 2px;
}

.grid-item-7 {
  border-width: 2px 2px 0 0;
}

.grid-item-8 {
  border-width: 2px 2px 0 2px;
}

.grid-item-9 {
  border-width: 2px 0 0 2px;
}
</style>
