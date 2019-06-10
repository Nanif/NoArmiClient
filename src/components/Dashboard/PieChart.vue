<script>
/* eslint-disable */

    import {Pie} from 'vue-chartjs'

    export default {
        extends: Pie,
        props: {
            finished: '',
            notFinished: ''
        },
        computed: {
            finishedText() {
                return ` מתוך ${this.sumStudents} הושלמו `
            },
            notFinishedText() {
                return ` מתוך ${this.sumStudents} נותרו `
            },
            sumStudents() {
                return this.finished + this.notFinished
            }
        },

        mounted: function () {
            this.renderChart({
                    type: 'pie',
                    labels: [this.finishedText, this.notFinishedText],
                    datasets: [
                        {
                            backgroundColor: ['#86e780', '#ff8080'],
                            data: [this.finished, this.notFinished],
                            borderWidth: 0.5,
                            hoverBackgroundColor: ['#6ddf66', '#ec3f46']

                        }
                    ]
                },
                {
                    legend: { //hides the legend
                        display: false
                    },
                    onClick: function () {
                        debugger
                    }

                })
        }
    }
</script>

<style scoped>
    .chartjs-render-monitor {
    }
</style>
