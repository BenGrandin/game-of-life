<template>
  <div  class="cell"
     v-bind:class="{ alive:isAlive}">
    {{message}}
  </div>
</template>

<script>

export default {
  name: 'cell',
  props:{
    message:String,
    isAlive:Boolean
  }
}
</script>


<style>
.cell {
  height: 10px;
  width: 10px;
  border: 1px solid black;
}
.alive {
  background-color: black;
}
</style>
