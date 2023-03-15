<template>
  <div id="app">
    <p> {{house}}</p>
    <button @click="trenches" style="background-color: red"> MAINLAND </button>
    <button @click="manipulate" style="background-color: blue;"> ISLAND </button>

  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  data(){
    return{
      house: "iyana Ipaja"
    }
  },
  methods:{
    manipulate(){
      this.house = "lekki phase one"
    },
    trenches(){
      this.house = "Akute Ogun STATE"
    }

  },
  components: {
    HelloWorld
  }
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
