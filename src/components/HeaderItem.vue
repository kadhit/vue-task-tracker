<template>
  <header>
    <h1>Task Tracker</h1>
    <ButtonItem
      @btn-click="$emit('toggle-add-task')"
      :text="showAddTask ? 'Close' : 'Add Task'"
      :color="showAddTask ? 'red' : 'green'"
    />
  </header>
</template>

<script>
  import ButtonItem from "./ButtonItem.vue";

  export default {
    name: "HeaderItem",
    props: {
      title: {
        type: String,
        default: "Hello World",
      },
      showAddTask: {
        type: Boolean,
      },
    },
    components: {
      ButtonItem,
    },
  };
</script>

<style scoped>
  header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
  }
</style>
