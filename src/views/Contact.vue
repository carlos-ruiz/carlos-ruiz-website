<template>
  <h1>Contact {{ msg }}</h1>
  <span>Computed: {{ testComputed }}</span>
</template>
<script lang="ts">
  import { defineComponent } from 'vue'
  export default defineComponent({
    data() {
      return {
        msg: 'message',
      }
    },
    computed: {
      testComputed(): string {
        return 'computed ' + this.msg
      },
    },
  })
</script>
