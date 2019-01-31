<template>

    <div class="container">
        <chart msg="1"/>

        <chart msg="2"/>

        <chart msg="3"/>

        <chart msg="4"/>
    </div>

</template>

<script>
    import chart from './components/Chart.vue'

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

    .container {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
        grid-gap: 5px;
    }
</style>
