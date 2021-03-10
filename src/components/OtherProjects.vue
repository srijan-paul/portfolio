<template>
  <div class="other-projects">
    <h3>What else?</h3>

    <p>Here are some other smaller projects I've made :)</p>

    <div class="other-projects-list">
      <ProjectCardSmall
        title="Sharpy Bot"
        :labels="['Typescript', 'DiscordJS']"
        link="https://github.com/srijan-paul/loveAnim"
      >
        A Discord Bot that can conduct quizzes, maintain user reputation, display leaderboards, show
        fun facts, cute animal pics and more!
      </ProjectCardSmall>

      <ProjectCardSmall
        title="Bonkyon"
        :labels="['Love2D', 'Lua']"
        link="https://github.com/srijan-paul/bonkyon"
      >
        A topdown turn based puzzle game written in Love2D. The player controls two minions
        simultaneously to solve puzzles. Play <a href="https://injuly.itch.io/bonkyon">here</a>.
      </ProjectCardSmall>

      <ProjectCardSmall
        title="LoveAnim"
        :labels="['Love2D', 'Lua']"
        link="https://github.com/srijan-paul/loveAnim"
      >
        A small animation library for the Love2D game engine. LoveAnim can create character
        animations from texture atlases.
      </ProjectCardSmall>
    </div>
  </div>
</template>

<script>
import ProjectCardSmall from "@/components/ProjectCardSmall.vue";

export default {
  components: {
    ProjectCardSmall,
  },
};
</script>

<style scoped>
.other-projects-list {
  display: flex;
  flex-direction: row;
  align-items: flex-start;
  justify-content: space-evenly;
  gap: 2%;
}

@media only screen and (max-width: 600px) {
  .other-projects-list{
    flex-direction: column;
    padding-left: 2%;
  }
}

</style>
