<template>
  <header>
    <div class="title">
      <h1>Social Media Dashboard</h1>
      <p>Total Followers: 23,004</p>
    </div>
    <div class="btn-radio" >
      <p>Dark Mode</p>
      <label class="switch">
        <input type="checkbox">
        <span class="slider round" @click="backgroundSwitcher"></span>
      </label>
    </div>
  </header>
</template>

<script>
export default {
  data () {
    return {
      isDark: false
    }
  },
  methods: {
    backgroundSwitcher () {
      if (this.isDark === false) {
        document.body.style.backgroundColor = 'hsl(230, 17%, 14%)'
        document.body.style.color = 'white'
        for (let i = 0; i < 4; i++) {
          document.querySelectorAll('.card')[i].style.backgroundColor = 'hsl(228, 28%, 20%)'
          document.querySelectorAll('.card h1')[i].style.color = 'white'
        }
        for (let i = 0; i < 8; i++) {
          document.querySelectorAll('.card-sm')[i].style.backgroundColor = 'hsl(228, 28%, 20%)'
          document.querySelectorAll('.card-sm .head p')[i].style.color = 'hsl(228, 34%, 66%)'
          document.querySelectorAll('.card-sm .numbers h1')[i].style.color = 'white'
        }
        this.isDark = true
      } else {
        document.body.style.backgroundColor = 'white'
        document.body.style.color = 'hsl(230, 17%, 14%)'
        for (let i = 0; i < 4; i++) {
          document.querySelectorAll('.card')[i].style.backgroundColor = 'hsl(225, 100%, 98%)'
          document.querySelectorAll('.card h1')[i].style.color = 'hsl(230, 17%, 14%)'  
        }
        for (let i = 0; i < 8; i++) {
          document.querySelectorAll('.card-sm')[i].style.backgroundColor = 'hsl(225, 100%, 98%)'
          document.querySelectorAll('.card-sm .head p')[i].style.color = 'hsl(228, 34%, 66%)'
          document.querySelectorAll('.card-sm .numbers h1')[i].style.color = 'hsl(230, 17%, 14%)'
        }
        this.isDark = false
      }
    }
  }
}
</script>

<style src="../style.css">

</style>