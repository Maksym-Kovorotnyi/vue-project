<template>
<div>
  <h1>{{ title }}</h1>
  <ButtonMain @click="incriment">Enter</ButtonMain>
</div>
</template>

<script>
import  ButtonMain  from './components/Button/Button-main.vue'

export default {
  name: 'App',
  components: {
    ButtonMain
  },
  data() {
    return {
      amountOfClicks: 0
    }
  },
  computed: {
    title() {
      return `amount of clicks ${this.amountOfClicks}`
    }
  },
  methods: {
    incriment() {
      this.amountOfClicks += 1
    }
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
