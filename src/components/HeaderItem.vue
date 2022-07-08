<template>
  <header>
    <h1>Task Tracker</h1>
    <ButtonItem text="Add Task" color="green"/>
  </header>
</template>

<script>
import ButtonItem from './ButtonItem.vue'

export default {
  name: 'HeaderItem',
  props: {
    title: {
      type: String,
      default: 'Hello World'
    }
  },
  components: {
    ButtonItem,
  }
}
</script>

<style scoped>
  header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
  }
</style>