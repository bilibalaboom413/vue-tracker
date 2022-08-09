<template>
  <header>
    <h1>{{ title }}</h1>
    <Button text="Add Task" color="green" />
  </header>
</template>

<script>
import Button from './Button'

  export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: 'Header',
    props: {
      title: {
        type: String,
      }
    },
    components: {
      Button,
    }
  }
</script>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-content: center;
  margin-bottom: 20px;
}
</style>