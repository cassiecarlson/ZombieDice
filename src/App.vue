<template>
  <div id="app">
    <dice></dice>
  </div>
</template>

<script>
import Hello from './components/Hello'
import Dice from './components/Dice'

export default {
  components: {
    Hello,
    Dice
  }
}
</script>

<style>
body {
  font-family: Helvetica, sans-serif;
}
</style>
