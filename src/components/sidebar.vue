<template>
  <div class="sidebar">
    <router-link to="/"><img alt="NodeBrew Logo" src="../assets/Logo.svg"></router-link>
    <h1>{{ title }}</h1>
    <p>{{ description }}</p>
    <nav-menu></nav-menu>
  </div>
</template>

<script>
import NavMenu from "./nav-menu";

export default {
  name: "Sidebar",
  components: {
    NavMenu
  },
  props: {
    title: String,
    description: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

.sidebar {
  background: $gray;
  height: 100%;
  text-align: center;
  padding: 3.5rem 2rem;
  box-sizing: border-box;

    img {
      height: 90px;
    }

    p {
      width: 80%;
      margin: 0 auto;
    }

}

</style>
