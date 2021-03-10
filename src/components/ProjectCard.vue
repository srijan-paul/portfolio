<template>
  <div class="project-card">
    <span class="card-title">{{ title }}</span>
    <div class="project-labels">
      <span v-for="label in labels" :key="label.name" :class="'project-label ' + label.className">
        {{ label.name }}
      </span>
      <!-- <span :class="'project-label ' + labelName">Typescript</span> -->
    </div>
    <p><slot>Project description missing</slot></p>
    <Button name="Github" :url="link" />
  </div>
</template>

<script>
import Button from "@/components/Button";

export default {
  props: {
    title: { type: String, required: true },
    link: { type: String, required: true },
    labels: { type: Array, required: true },
  },
  components: {
    Button,
  },
};
</script>

<style scoped>
.project-card {
  text-align: left;
  border-radius: 2%;
  padding: 3%;
  box-shadow: -1px 3px 23px -11px rgba(179, 168, 175, 1);
  margin-bottom: 5%;
  background-color: #ffffff;
}

.project-labels {
  padding: 1% 0 1% 0;
}

.project-label {
  font-size: 80%;
  margin-right: 1%;
  padding: 0.1% 1%;
  opacity: 0.8;
}

.label-ts {
  color: white;
  background-color: #007acc;
}

.label-js {
  color: black;
  background-color: #f0db4f;
}

.label-node-js {
  color: white;
  background-color: #3c873a;
}

.label-c {
  color: white;
  background-color: #d9534f;
}

.label-lua {
  color: white;
  background-color: #53489b;
}

.label-love {
  color: white;
  background: #eb2484;
}

.project-label:hover {
  cursor: pointer;
  opacity: 1;
}

.card-title {
  font-weight: 700;
  text-decoration: underline var(--hlColor);
  font-size: 2.5rem;
}

@media only screen and (max-width: 600px) {
  .project-card {
    font-size: 1.5rem;
    padding: 5%;
  }
}
</style>
