<template>
  <button v-if="showClearCompletedButton"
          @click="clearCompleted">Kaldır</button>
</template>

<script>
    export default {
        name: "todo-clear-completed",
      props:{
        showClearCompletedButton:{
          type : Boolean,
          required: true,
          }
      },
      methods:{
        clearCompleted() {
          eventBus.$emit('clearCompletedTodos')
        }
      }
    }
</script>

<style scoped>

</style>
