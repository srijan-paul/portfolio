<template>
  <section id="app">
    <div class="wrapper">
      <DashBoard />
      <hr />
      <CardList />
      <hr />
      <Tools />
      <hr />
      <ProjectList />
      <hr />
      <OtherProjects />
      <hr />
      <Contact />
    </div>
    <Footer />
  </section>
</template>

<script>
import DashBoard from "@/components/DashBoard";
import ProjectList from "./components/ProjectList";
import CardList from "@/components/CardList";
import Tools from "@/components/Tools";
import Footer from "@/components/Footer";
import OtherProjects from "@/components/OtherProjects";
import Contact from "@/components/Contact";

export default {
  name: "App",
  components: {
    DashBoard,
    ProjectList,
    CardList,
    Tools,
    Footer,
    OtherProjects,
    Contact,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Fira+Code&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Inconsolata&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Roboto+Mono&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Noto+Sans&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Poppins&display=swap");

:root {
  --hlColor: #ee5253;
  --bgColor: #ffffff;
  --fgColor: #333333;
  --fontSans: "Poppins", "Calibre", "sans-serif";
}

body {
  margin: 0;
  padding: 0;
  font-family: "Roboto Mono", sans-serif;
  color: var(--fgColor);
  background-color: var(--bgColor);
}

h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: "Fira Code", sans-serif;
}

.section-title {
  font-family: "Roboto", sans-serif;
  font-weight: 700;
}

#app {
  margin: 5% auto 8%;
  margin-bottom: 3%;
}

.wrapper {
  width: 60%;
  margin: auto;
  font-size: 1.7rem;
  text-align: center;
}

@media only screen and (max-width: 600px) {
  .wrapper {
    width: 100%;
  }
  #app {
    width: 95%;
  }
}
</style>
