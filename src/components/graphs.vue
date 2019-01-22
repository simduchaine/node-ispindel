<template>
    <div id="graphs">
        <div id="lineChart" class="card">
            <h3>Plato, Temperature</h3>
            <line-chart style="height: 80%"></line-chart>
        </div>
        <card v-for="card in cards" :key="card.id" :title="card.title" :value="card.value" :unit="card.unit" :style="{color: card.color}"  class="card"></card>
    </div>
</template>

<script>
import lineChart from "./data-cards/line-chart"
import card from "./data-cards/card"

export default {
    name: "Graphs",
    components: {
        lineChart,
        card
    },
    data() {
        return {
            cards: [
                {id: 1, title: "Battery", value: 56, unit: "%"},
                {id: 2, title: "Tilt", value: 88.30, unit: "°", color: "#78E3D9"},
                {id: 3, title: "Gravity", value: 3.24, unit: "°p", color: "#F88782"},
                {id: 4, title: "Temperature", value: 25.53, unit: "°C", color: "#8F9BEC"}
            ]
        }
    }
    
}
</script>

<style lang="scss">

#lineChart {
    grid-column: 1 / 5;
} 

#graphs {
    display: grid;
    grid-template-rows: 400px 3fr;
    grid-template-columns: 1fr 1fr 1fr 1fr;
    grid-gap: 1.5em;

    h3 {
        color: $purple;
        font-size: 18px;
        font-weight: normal;
    }

    .card {
        box-shadow: 4px 4px 25px rgba(215, 217, 233, 0.59);
        border-radius: 10px;
        background: $card-bg;
        width: 100%;
        height: 100%;
        padding: 0.5em 1.5em;
        box-sizing: border-box;
        position: relative;
    }
}    
</style>