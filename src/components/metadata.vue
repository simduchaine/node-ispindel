<template>
    <div>
        <h1>Brewing: <span class="brewName">{{ brewName }}</span></h1>
    </div>
</template>

<script>
export default {
    name: "Metadata",
    computed: {
        brewName() {
            return this.$store.state.brewName;
        }
    }
    
}
</script>

<style scoped lang="scss">

h1 {
    color: $purple;
    font-size: $medium-size;
}

.brewName {
    color: $font-color;
    font-weight: normal;
    padding-left: 0.5em;
}
    
</style>