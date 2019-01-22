
<script>
import { Line } from "vue-chartjs"

Chart.defaults.global.defaultFontColor = "#8488b1";
Chart.defaults.global.defaultFontFamily = "PT Sans";
Chart.defaults.global.legend.labels.usePointStyle = true;

export default {
    extends: Line,
    mounted () {
        this.renderChart({
        labels: ["January", "February", "March", "April", "May", "June", "July"],
        datasets: [
            {
                label: "Plato°",
                borderColor: "#8F9BEC",
                backgroundColor: "#8F9BEC",
                fill: false,
                data: [40, 39, 10, 40, 39, 80, 40],
                yAxisID: "y1"
            },
            {
                label: "Temperature (°C)",
                borderColor: "#F88782",
                backgroundColor: "#F88782",
                fill: false,
                data: [60, 55, 32, 10, 2, 12, 53],
                yAxisID: "y2"
            }
        ]
        }, 
        {
            responsive: true, 
            maintainAspectRatio: false, 
            fontFamily: "PT Sans",
            scales: {
                yAxes: [{
                    id: "y1",
                    type: "linear",
                    position: "left"
                }, {
                    id: "y2",
                    type: "linear",
                    position: "right",
                    gridLines: {
                        display: false
                    }
                }]
            }
        })
    }
    
}
</script>