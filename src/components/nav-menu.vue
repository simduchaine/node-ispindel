<template>
    <div id="nav">
      <ul>
        <li><a href="#"><font-awesome-icon icon="plus-circle" class="icon" />New Brew</a></li>
        <li><a href="#"><font-awesome-icon icon="file-excel" class="icon"/>Download Data</a></li>
        <li><a href="#"><font-awesome-icon icon="edit" class="icon"/>Edit Data</a></li>
      </ul>
    </div>
</template>

<script>
export default {
  
};
</script>

<style scoped lang="scss">

#nav {
  margin-top: 3rem;

  ul {
    list-style-type: none;

    li {
      display: block;
      text-align: left;
      padding: 0.5em 0;

      a {
        .icon {
        color: #bfbfbf;
        padding-right: 0.5em;
        }

        &:hover {
          color:  $h-color;

          .icon {
            color: #737CBE;
          }
        }
      }
    }
    
  }
}
    
</style>
