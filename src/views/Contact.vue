<template>
  <h1>Contact {{ msg }}</h1>
  <span>Contact information: {{ testComputed }}</span>
</template>
<script lang="ts">
  import { defineComponent } from 'vue'
  export default defineComponent({
    data() {
      return {
        msg: 'to be defined',
      }
    },
    computed: {
      testComputed(): string {
        return 'Info ' + this.msg
      },
    },
  })
</script>
