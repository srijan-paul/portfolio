<template>
  <div class="tools-list">
    <h3>Stuff I work with</h3>

    <div class="tool-title">Languages</div>
    <div class="tool-icons">
      <Icon name="cpp.svg" size="40" text="C++" />
      <Icon name="lua.svg" size="40" text="Lua" />
      <Icon name="typescript.svg" size="40" text="Typescript" />
      <Icon name="javascript.svg" size="40" text="Javascript " />
      <!-- credit: https://freeicons.io/vector-and-svg-logos-icons-15/python-icon-8940 -->
      <Icon name="python.svg" size="40" text="Python" />
    </div>

    <div class="tool-title">Frameworks / Services</div>
    <div class="tool-icons">
      <Icon name="love2d.png" size="40" text="Love2D" />
      <Icon name="react.svg" size="40" text="React" />
      <Icon name="nodejs.svg" size="40" text="NodeJS" />
      <Icon name="express.svg" size="40" text="Express" />
      <!-- credit: https://freeicons.io/vector-and-svg-logos-icons-17/sass-icon-9036 -->
      <Icon name="sass.svg" size="40" text="Sass" />
      <!-- credit: https://freeicons.io/vector-and-svg-logos-icons-08/firebase-icon-icon -->
      <Icon name="firebase.svg" size="40" text="Firebase" />
    </div>
  </div>
</template>

<script>
import Icon from "@/components/Icon";
export default {
  components: { Icon },
};
</script>

<style scoped>
.tools-list .icon {
  margin: 10px;
}

.tool-title {
  font-size: 2rem;
  margin-bottom: 2%;
  color: #999;
}
</style>
