<template>
  <div id="app">
    <div id="nav">
      <router-link to="/"><img alt="Vue logo" src="./assets/Logo.svg"></router-link>
    </div>
    <router-view/>
  </div>
</template>

<style lang="scss">

@import url('https://fonts.googleapis.com/css?family=PT+Sans:400,700');

$font: 'PT Sans', sans-serif;
$font-color: #8488B1;
$h-color: #353B4B;
$bg: #F6F6FC;
$shadow: 4px 4px 25px rgba(215, 217, 233, 0.59);

#app {
  font-family: $font;
  color: $font-color;
  width: 80%;
  height: 85%;
  margin: 0 auto;
  background: $bg;
  opacity: 0.9;
  box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.13);

}

</style>
