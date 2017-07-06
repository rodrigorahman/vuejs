<template>
  <section id="todoapp">
    <header class="header">
      <h1>Tarefas</h1>
      <input-task></input-task>
    </header>
  </section>
</template>

<script>
  import InputTask from './components/InputTask'
  export default {
    name: 'app',
    components: {
      InputTask
    }
  }
</script>

<style>
  #todoapp {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
</style>
