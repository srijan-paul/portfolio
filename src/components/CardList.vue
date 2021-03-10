<template>
  <div class="card-list">
    <h3>Interests</h3>
    <div class="cards">
      <Card title="Compiler design" icon="compiler">
        Compilers are the CS subject I'm the most interested in. I've written several toy
        programming languages over the course of my learning. As of late, I've been developing a
        more "serious" programming language project that you can find below, or on my github. My
        favorite tools for this are C/C++. I used to be a stickler for C but lately I've come to
        find C++'s improvements worthwhile, safe and time saving.
      </Card>

      <Card title="Web" icon="web">
        I look into Web dev every now and then. VueJS is my tool of choice for front ends, It hits
        the perfect balance between sufficient tooling and minimalism. If I'm not using Vue then I'm
        most likely just using vanilla HTML and CSS/SASS. For the backend- Express, NodeJS and
        Firebase usually satisfy my needs.
      </Card>

      <Card title="Gamedev" icon="game">
        It's always a joy to try out the fun games that indie studios and individuals come up with.
        Following from there, I also enjoy game development as a hobby. I've tried a bit of several
        toolchains and engines, but my favorite will always be
        <a href="https://love2d.org/">LOVE2D</a>. The fact that it uses Lua as a scripting language
        is ofcourse a big bonus on top of it's design :)
      </Card>
    </div>
  </div>
</template>

<script>
import Card from "@/components/Card";
export default {
  components: { Card },
};
</script>

<style scoped>
.cards {
  margin-top: 5%;
  display: grid;
  gap: 4rem;
  grid-template-columns: 1fr 1fr;
}

@media only screen and (max-width: 1000px) {
  .cards {
    grid-template-columns: 1fr;
  }
}

a {
  font-weight: bolder;
  color: var(--hlColor);
}
</style>
