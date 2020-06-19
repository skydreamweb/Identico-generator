<template>
  <div class="hello">
    <h1>{{ msg }}</h1> 
      Input:
    <input @input="onInput" type="text">

  </div>
</template>

<script>
export default {
  name: 'Input',
  props: {
    msg: String
  },
  methods: {
    onInput: function(e) {
      console.log(e.target.value);
      
      
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
