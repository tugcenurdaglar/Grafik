<template>
    <div>
        <highcharts class="hc" :options="chartOptions" ref="chart"></highcharts>
    </div>
</template>

<script>
    export default {
        name: "Chart",
        data() {
            return {
                chartOptions: {
                    series: [
                        {
                            data: [1, 2, 3]
                        }
                    ]
                }
            };
        }
    };
</script>

<style scoped>

</style>