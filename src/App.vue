<template>
  <div class="top_container">
    <img class="logo" src="./img/logo.png" alt="logo" />
    <p class="name">KIND_KILLERWHALE</p>
    <img class="logo2" src="./img/kuromi2.png" alt="kuromi" />
  </div>

  <Profile />
  <ProjectComponent />
</template>

<script>
import Profile from "./components/profile.vue";
import ProjectComponent from "./components/projects.vue";

export default {
  name: "App",
  components: {
    Profile,
    ProjectComponent,
  },
};
</script>

<style>
body {
  background-color: #fbdff0;
  user-select: none;
  height: 5000px;
}

.top_container {
  background-color: black;
  margin: -10px;
  padding-top: 20px;
  height: 400px;
  text-align: center;
}

.logo {
  width: 150px;
}

.name {
  color: white;
  font-family: "marvin-round", "sans-serif";
  font-size: 35px;
  margin: 20px;
}

.logo2 {
  width: 150px;
}
</style>
