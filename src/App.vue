<template>

    <div class="container">
        <chart chartsize="chart-item"/>
        <chart chartsize="chart-item"/>
        <chart chartsize="chart-item"/>
        <chart chartsize="chart-item"/>
        <chart chartsize="chart-item"/>
        <chart chartsize="chart-item"/>
        <chart chartsize="chart-item"/>
        <chart chartsize="chart-item"/>
        <chart chartsize="chart-item"/>
        <chart chartsize="chart-item"/>
    </div>

</template>

<script>
    import chart from './components/MyChart.vue'

    export default {
        name: 'app',
        components: {
            chart
        }
    }
</script>

<style>
    #app {
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
        margin-top: 60px;
    }

    .chart-item {
        height: 100%;
    }

    .wrap {
        min-width: 0;
    }


    .container {
        display: grid;
        grid-template-columns: repeat(12, auto);
        grid-template-rows: auto;
        height: 100vh;
    }

    .container .wrap:nth-child(1) {
        grid-column: span 6;
        grid-row: span 2;
        height: 100%;
    }

    .container .wrap:nth-child(2) {
        grid-column: span 3;
        height: 100%;
    }

    .container .wrap:nth-child(3) {
        grid-column: span 3;
        height: 100%;
    }

    .container .wrap:nth-child(4) {
        grid-column: span 3;
        height: 100%;
    }

    .container .wrap:nth-child(5) {
        grid-column: span 3;
        height: 100%;
    }

    .container .wrap:nth-child(6) {
        grid-column: span 3;
        height: 100%;
    }

    .container .wrap:nth-child(7) {
        grid-column: span 3;
        height: 100%;
    }

    .container .wrap:nth-child(8) {
        grid-column: span 2;
        height: 100%;
    }

    .container .wrap:nth-child(9) {
        grid-column: span 2;
        height: 100%;
    }

    .container .wrap:nth-child(10) {
        grid-column: span 2;
        height: 100%;
    }

</style>
