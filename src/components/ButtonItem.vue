<template>
  <button class="btn" @click="onClick()" :style="{background: color}">{{ text }}</button>
</template>

<script>
  export default {
    name: 'ButtonItem',
    props: {
      text: {
        type: String,
        default: 'Button'
      },
      color: {
        type: String,
        default: '#c0c0c0',
      },
    },
    methods: {
      onClick() {
        console.log('click');
      }
    }
  }
</script>