<template>
  <div>
    <button
    class="btn"
    :style="{ background: color }"
    @click="onClick()">{{text}}</button>
  </div>
</template>

<script>
  export default {
    name: 'Button',
    data: () => ({
    }),
    props: {
      text: {
        type: String,
      },
      color: {
        type: String,
      }
    },
    methods: {
      onClick() {
        this.$emit('btn-click')
      }
    }
  }
</script>

<style scoped>
</style>
