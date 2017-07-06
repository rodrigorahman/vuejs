<template>
  <div>
    <input class="new-todo"
           v-on:keyup="addTask"
           placeholder="O que precisa ser feito?">
  </div>
</template>

<script>

  import { Task } from '../models/Task'

  export default {
    data () {
      return {}
    },
    methods: {
      addTask (value) {
        let task = new Task()
        task.completed = false
        task.title = value
      }
    }
  }
</script>

<style>

</style>
