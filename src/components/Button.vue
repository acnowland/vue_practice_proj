<template>
  <button @click="onClick()" :style="{ background: color }" class="btn">
    {{ text }}
  </button>
</template>

<script>
export default {
  name: "Button",
  props: {
    color: String,
    text: String,
    showAddTask: Boolean
  },
  methods: {
    onClick() {
      this.$emit('toggle-button')
    },
  },
};
</script>
