<template>
  <div id="app">
    <navigator></navigator>
    <div class="big-card">
      <bigcards></bigcards>
    </div>
    <h2>Overview - Today</h2>
    <div class="lt-cards">
      <littlecards></littlecards>
    </div>
  </div>
</template>

<script>
import Navigator from './components/Navigator.vue'
import Bigcards from './components/Bigcards.vue'
import Littlecards from './components/Littlecards.vue'

export default {
  name: 'App',
  components: {
    Navigator, 
    Bigcards,
    Littlecards
  }
}
</script>

<style src="./style.css">
</style>
