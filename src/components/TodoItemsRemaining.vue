<template>
  <div>{{ remaining }} kalan</div>
</template>

<script>
    export default {
        name: "todo-remaining",
        props:{
          remaining:{
            type:Number,
            required:true
          }
      }
    }
</script>

<style scoped>

</style>
