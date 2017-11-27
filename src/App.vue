<template>
  <div id="app">
    <h1>{{ msg }}</h1>
    <datetime
        v-model="date1"
        type="date"
        input-format="DD-MM-YYYY"
        placeholder="Select date"
        moment-locale="zh-cn">
    </datetime>
    <datetime
        v-model="date2"
        type="date"
        input-format="DD-MM-YYYY"
        placeholder="Select date"
        locale="zh-cn">
    </datetime>
  </div>
</template>

<script>
  import { Datetime } from 'vue-datetime'

  export default {
    name: 'app',
    data () {
      return {
        date1: '',
        date2: '',
        msg: 'Welcome to Your Vue.js App'
      }
    },
    components: {
      Datetime
    }
  }
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
