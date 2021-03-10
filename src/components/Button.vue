<template>
  <a :href="url" target="_blank">
    <div class="button">
      {{ name }}
    </div>
  </a>
</template>

<script>
export default {
  name: "Button",
  props: {
    name: {
      type: String,
      required: true,
    },
    url: String,
  },
};
</script>

<style scoped>
.button {
  color: black;
}

a {
  color: inherit;
  text-decoration: inherit;
  outline: none;
}

.button:hover {
  color: white;
  background-color: var(--hlColor);
  border-color: var(--hlColor);
  transition-duration: 300ms;
}
</style>
