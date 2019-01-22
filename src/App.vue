<template>
  <div id="app">
    <sidebar title="BrewNode" description="iSpindel Electronic Hydrometer Dashboard"/>
    <router-view/>
  </div>
</template>

<script>
import sidebar from "@/components/sidebar.vue";

export default {
  components: {
    sidebar
  }
}
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css?family=PT+Sans:400,700");

#app {
  font-family: $font;
  color: $font-color;
  font-size: $normal-size;
  width: 80%;
  height: 88%;
  margin: 0 auto;
  background: $bg;
  box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.13);
  display: grid;
  grid-template-columns: 20% auto;
}

h1 {
  color: $h-color;
  font-weight: bold;
  font-size: $big-size;
}

a {
  color: inherit;
  text-decoration: none;
}

</style>
