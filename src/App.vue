<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <input v-model="option" placeholder="Enter something" />
  <button @click="myfunction">Click me</button>
  <HelloWorld 
    :msg="mymessage" 
    :mylist="myiiemlist"
  />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  data() {
    return {
      mymessage:"hello world",
      myiiemlist: [],
      option: ''
    }
  },
  methods:{
    myfunction(){
      if (this.option == '1'){
        this.myiiemlist= ['Item 1' , 'Item 2', 'Item 3', 'Item 4', 'Item 5', 'Item 6', 'Item 7']
      }
      else{
        this.myiiemlist= []
      }
    }
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
