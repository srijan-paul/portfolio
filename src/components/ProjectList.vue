<template>
  <div class="projects">
    <h2>Projects</h2>
    <div class="project-list">
      <ProjectCard
        title="Ave"
        link="https://github.com/srijan-paul/AveTS"
        :labels="[
          { name: 'Typescript', className: 'label-ts' },
          { name: 'Javascript', className: 'label-js' },
          { name: 'Node JS', className: 'label-node-js' },
        ]"
      >
        A statically type checked programming language that compiles to Javascript. It is very
        similar to typescript, but with minimal whitespace sensitive syntax like Python. Ave aims to
        be a blend between Coffeescript and Typescript, providing both type safety and noise free
        syntax.
      </ProjectCard>

      <ProjectCard
        title="Snap"
        link="https://github.com/srijan-paul/snap"
        :labels="[{ name: 'C++', className: 'label-c' }]"
      >
        An interpreted, dynamically typed programming language inspired by Lua. The Snap VM is
        highly inspired by LuaVM's design. The goal was to provide the minimalism of Lua, but with
        some syntactic sugar to aid Programmers that are used to JS/C.
        <br />
        <br />
        Snap picks up almost all of Lua's features and adds support for OOP, compound assignment
        operators and some more QoL features. The VM can be embedded in C++ applications like Game
        engines.
      </ProjectCard>

      <ProjectCard
        title="Shriek"
        link="https://github.com/srijan-paul/horror-game"
        :labels="[
          { name: 'Lua', className: 'label-lua' },
          { name: 'Love2D', className: 'label-love' },
        ]"
      >
        A topdown RPG horror game written using the Love2D game engine. Shriek is an atmospheric and
        story driven horror game inspired by Indie games like Last Train Home and No Delivery. The
        Game is in a playable state but still a Work In Progress at the moment.
      </ProjectCard>

      <ProjectCard
        title="JSONC"
        link="https://github.com/srijan-paul/json-parser"
        :labels="[{ name: 'C', className: 'label-c' }]"
      >
        A fast and simple JSON parser written in C. JSONC makes it extremely simple to load JSON
        data from files and strings into your C and C++ projects.
      </ProjectCard>
    </div>
  </div>
</template>

<script>
import ProjectCard from "@/components/ProjectCard";
export default { components: { ProjectCard } };
</script>

<style scoped>
.projects {
  margin-top: 4%;
}
</style>
