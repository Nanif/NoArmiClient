<template>
    <div>
        <div class="container">
            <div class="charts">
                <pie-chart :finished="20" :not-finished="12" class="pieChart" id="exemption"></pie-chart>
                <pie-chart :finished="20" :not-finished="8" class="pieChart" id="decleration"></pie-chart>
                <pie-chart :finished="20" :not-finished="2" class="pieChart" id="TZ"></pie-chart>
            </div>
            <groups></groups>
            <dashboard></dashboard>
          <side-bar></side-bar>
        </div>
    </div>
</template>

<script>
    import Dashboard from '../Dashboard/Dashboard'
    import groups from '../Dashboard/Groups'
    import PieChart from '../Dashboard/PieChart'
    import SideBar from "../Actions/SideBar";

    export default {
        name: 'Index.vue',
        components: {
          SideBar,
            Dashboard,
            PieChart,
            groups
        }
    }
</script>

<style lang="scss" scoped>
    .charts {
        display: flex;
        justify-content: space-between;
        width: 950px;
        margin: auto;

        .pieChart {
            width: 120px;
            height: 120px;
        }
    }
</style>
