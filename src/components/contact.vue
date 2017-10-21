<template>
    <div class="hello">
        <h1>{{ msg }}</h1>
        <p>{{ message }}</p>
        <input v-model="message">
    </div>
</template>

<script>
  let data = {
    msg: 'CONTACT',
    message: 'Hallo Welt'
  }

  export default {
    name: 'Contact',
    data () {
      return data
    },
    created: function () {
      // `this` points to the vm instance
      console.log('message is: ' + this.message)
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>



</style>
