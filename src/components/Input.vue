  
<template>
  <div>
    <h3>Input text:</h3>
    <input type='text' @input='onInput' />
    <h3>Your identicon:</h3>
    <div v-html='identicon'></div>
  </div>
</template>
<script>
import jdenticon from 'jdenticon';
export default {
    data() {
      return {
        textInput: ''
      }
    },
    computed: {
      identicon: function() {
        return jdenticon.toSvg(this.textInput, 200);
      }
    },
    methods: {
      onInput: function(event) {
        this.textInput = event.target.value;
      }
    }
}
</script>
<style>
</style>
