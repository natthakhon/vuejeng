<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    {{ mylist.length }}
    <ul>
      <li v-for="(item, index) in mylist" :key="index">
        {{ item }}
      </li>
    </ul>    
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
    mylist:{               
      type: Array,
      required: true,
      default: () => []
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
