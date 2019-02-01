<template>
    <div class="wrap">
        <line-chart :chartdata="chartData" :options="options" v-bind="chart"></line-chart>
    </div>
</template>

<script>
    import LineChart from '@/components/Chart.js'

    export default {
        name: 'chart',
        components: {
            LineChart
        },
        props: { chartsize: String },
        data() {
            return {
                chart: {
                    cssClasses: this.chartsize
                },
                chartData: {
                    labels: ["Red", "Blue", "Yellow", "Green", "Purple", "Orange"],
                    datasets: [{
                        label: '# of Votes',
                        data: [12, 19, 3, 5, 2, 3]
                    }]
                },
                options: {
                    responsive: true,
                    maintainAspectRatio: false
                }
            }
        }
    }
</script>

<style>

</style>
