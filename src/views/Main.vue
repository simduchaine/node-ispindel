<template>
  <div class="home">
    <HelloWorld msg="Node iSpindel App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "main",
  components: {
    HelloWorld
  }
};
</script>
