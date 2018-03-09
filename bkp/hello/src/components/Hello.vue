<template>
  <div class="hello">
    <h1 :title="msg">{{ msg }}</h1>
  </div>
</template>

<script>
  export default{
    name: 'hello',
    data () {
      return {
        msg: 'Bem vindo a sua primeira app com Vue.js'
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
