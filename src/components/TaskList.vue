<template>
  <div :key="task.id" v-for="task in tasks">
    <TaskItem :task="task" />
  </div>
</template>
<script>
import TaskItem from './TaskItem.vue';

export default {
  name: "TaskList",
  props: {
    tasks: {
      type: Array,
    },
  },
  components: {
    TaskItem
  }
};
</script>
