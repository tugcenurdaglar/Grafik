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
                    chart: {
                        type: 'pie'
                    },
                    series: [
                        {
                            innerSize: '50%',

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