<template>
  <div id='app'>
    <p>Find me in app/javascript/components/app.vue</p>
    Type in your message:
    <input type="text" id="input1" v-model="message" size="50">
    <p>The value of the input is: {{ message }}</p>
    <ul>
      <li v-for="name in names" v-text="name"></li>
    </ul>
    <input type="text" id="input2">
    <button v-on:click="onClick ">Add Name</button>
  </div>
</template>

<script>
  export default {
    data: function () {
      return {
        message: "Welcome to Cinematronix!",
        names: ['Joe', 'Mary', 'Jane', 'Jack ']
      }
    }
  }
</script>

<style scoped>
  p {
    font-size: 2em;
    text-align: center;
  }
  #input {
    font-size: 4em;
  }
</style>
