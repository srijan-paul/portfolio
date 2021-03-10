<template>
  <div class="project-card-small">
    <div class="row-top">
      <img :src="require(`../assets/folder.svg`)" width="28" height="28" />
      <h5 class="project-small-title">{{ title }}</h5>
    </div>

    <div class="project-small-description">
      <slot>
        Project description missing
      </slot>
    </div>

    <div class="project-small-labels">
      <span v-for="label in labels" :key="label" class="project-small-label">
        {{ label }}
      </span>
    </div>

    <div>
      <a :href="link"><span class="btn">Github</span></a>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: { type: String, required: true },
    labels: { type: Array },
    link: { type: String },
  },
};
</script>

<style scoped>
.project-card-small {
  flex: 33%;
  text-align: left;
  border-radius: 2%;
  padding: 3%;
  box-shadow: -1px 3px 23px -11px rgba(179, 168, 175, 1);
  margin-bottom: 5%;
  background-color: #ffffff;
}

.project-small-title {
  padding-left: 10%;
  font-weight: bolder;
  font-family: var(--fontSans);
  display: inline-block;
}

a {
  text-decoration: inherit;
  color: inherit;
  opacity: 0.8;
}

a:hover {
  opacity: 1.0;
}

.row-top {
  display: flex;
}

.project-small-description {
  font-size: 90%;
  text-align: left;
}

.project-small-label {
  opacity: 0.8;
  padding-right: 5%;
}

.project-small-labels {
  font-size: 80%;
  margin-top: 6%;
}

.btn {
  text-decoration: underline;
  text-decoration-thickness: 3px;
  text-decoration-color: var(--hlColor);
}

.btn:hover {
  cursor: pointer;
}

@media only screen and (max-width: 600px) {
  .row-top{
   padding: 2%; 
  }
}
</style>
