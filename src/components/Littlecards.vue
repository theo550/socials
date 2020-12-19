<template>
  <div class="card-control">
    <views></views>
    <likes></likes>
  </div>
</template>

<script>

import Views from './Views.vue'
import Likes from './Likes.vue'


export default {
  components: {
    Views,
    Likes
  },
}
</script>

<style src="../style.css">

</style>