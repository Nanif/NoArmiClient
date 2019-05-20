<template>
    <div>
        <ul class="nav nav-tabs" dir="rtl" id="ul_group_nav">
            <li :key="index" @click="changeActiveGroup(index)" class="nav-item" v-for="(group,index) in groupsList">
                <a :class="{'active': group.isActive}" class="nav-link"
                   data-toggle="tab" href="#home" role="tab"><span>{{ group.Displayname }}</span></a>
            </li>
        </ul>
    </div>
</template>

<script>
    export default {
        name: "groups",
        data() {
            return {
                groupsList: [
                    {
                        Displayname: 'קבוצת חורף',
                        isActive: true
                    },
                    {
                        Displayname: 'קבוצת אביב',
                        isActive: false
                    },{
                        Displayname: 'קבוצת סתו',
                        isActive: false
                    }, {
                        Displayname: 'קבוצת קיץ',
                        isActive: false
                    }
                ]
            }
        },
        methods: {
            changeActiveGroup(index) {
                this.groupsList.forEach(group => {
                    group.isActive = false;
                });
                this.groupsList[index].isActive = true;
            }
        }
    }
</script>

<style lang="scss" scoped>
    #ul_group_nav {
        padding: 0;
    }

    a {
        color: #515a62

    }

    .nav-link {
        border: solid 1px #e4e7ea;

        &.active {

            background-color: #f2f2f2;
        }
    }

</style>
