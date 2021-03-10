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
        title="Mad Carbon"
        link="https://github.com/srijan-paul/bullet_hell"
        :labels="[
          { name: 'Lua', className: 'label-lua' },
          { name: 'Love2D', className: 'label-love' },
        ]"
      >
        A retro bullet hell game written in Lua with the Love2D game framework. The player explores
        a dungeon filled with monsters, critters and treasures to reach the orb of truth. Offers a
        variety of weapons, items and a level editor that can be used to craft levels.
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
