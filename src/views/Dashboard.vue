<template>
  <div id="dashboard">
    <metadata></metadata>
    <graphs></graphs>
  </div>
</template>

<script>
// @ is an alias to /src
import metadata from "@/components/metadata.vue";
import graphs from "@/components/graphs.vue";

export default {
  name: "Dashboard",
  components: {
    metadata,
    graphs
  }
};
</script>

<style lang="scss">

#dashboard {
  display: grid;
  grid-template-rows: 10vh 1fr;
  padding: 2.5em 3em;
}
  
</style>