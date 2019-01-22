<template>
    <div>
        <h3>{{ title }}</h3>
        <div class="bigData">{{ value }}{{ unit }}</div>
    </div>
</template>

<script>
export default {
    name: "card",
    props: ["title", "value", "unit", "color"]
}
</script>

<style scoped lang="scss">

.bigData {
    font-size: 45px;
    font-weight: bold;
    text-align: center;
    padding-top: 0.5em;
}
    
</style>