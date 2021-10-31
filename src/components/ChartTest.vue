<template>
    <div class="chart">
        <div id="main" ref="main" style="height: 100%"></div>
    </div>
</template>
<script>
    import echarts from 'echarts';

    export default {
        name: 'lineChart',
        data() {
            return {
            };
        },
        mounted() {
            const myChart = echarts.init(this.$refs.main);
            const getNumber = this.getRandomNumber;

            myChart.setOption({
                // title: {
                //     text: 'ECharts entry example'
                // },
                tooltip: {},
                xAxis: {
                    data: ['A', 'B', 'C', 'D', 'E', 'F']
                },
                yAxis: {},
                series: [{
                    name: 'Test',
                    type: 'bar',
                    data: [getNumber(), getNumber(), getNumber(), getNumber(), getNumber(), getNumber()],
                    itemStyle: {
                        color: '#42b983',
                    },
                }]
            });
        },
        methods: {
            getRandomNumber() {
                return  Math.round(Math.random() * 100, 0);
            }
        }
    }

</script>
<style>
    .chart{
        width: 100%;
        height: 300px;
    }

</style>