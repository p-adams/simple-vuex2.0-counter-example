<template>
  <div id="app">
    <h3>The count: {{count}}</h3>
    <button @click="$store.dispatch('dec')">-</button>
    <button @click="$store.dispatch('inc')">+</button>
  </div>
</template>

<script>
export default {
  computed: {
    count(){
      return this.$store.state.count
    }
  }
}
</script>

<style>
body {
  font-family: Helvetica, sans-serif;
}
</style>
