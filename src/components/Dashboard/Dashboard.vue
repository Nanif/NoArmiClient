<template>
    <div>
        <!--        <font-awesome-icon icon="coffee"/>-->
        <table class="table table-responsive-md table-fixed  table-bordered table-striped" dir="rtl" id="tableFiles">
            <thead>
            <tr>
                <th v-for="field in studentsFields"> {{ field }}</th>
            </tr>
            </thead>

            <tbody>
            <tr v-for="student in students">
                <td>{{student.tz}}</td>
                <td>{{student.firstName}}</td>
                <td>{{student.lastName}}</td>
                <td>{{student.birthDate}}</td>
                <td>{{student.address}}</td>
                <td>{{student.phone}}</td>
            </tr>
            </tbody>
        </table>
    </div>
</template>

<script>
    export default {
        name: 'Dashboard',
        data() {
            return {
                students: [
                    {
                        tz: 207145244,
                        firstName: 'נעמי',
                        lastName: 'פישביין',
                        birthDate: '07/05/1998',
                        address: 'רשבם 22 בני ברק',
                        phone: '50411215',
                    },

                    {
                        tz: 207145244,
                        firstName: 'נעמי',
                        lastName: 'פישביין',
                        birthDate: '07/05/1998',
                        address: 'רשבם 22 בני ברק',
                        phone: '50411215',
                    },
                    {
                        tz: 207145244,
                        firstName: 'נעמי',
                        lastName: 'פישביין',
                        birthDate: '07/05/1998',
                        address: 'רשבם 22 בני ברק',
                        phone: '50411215',
                    },
                    {
                        tz: 207145244,
                        firstName: 'נעמי',
                        lastName: 'פישביין',
                        birthDate: '07/05/1998',
                        address: 'רשבם 22 בני ברק',
                        phone: '50411215',
                    },
                    {
                        tz: 207145244,
                        firstName: 'נעמי',
                        lastName: 'פישביין',
                        birthDate: '07/05/1998',
                        address: 'רשבם 22 בני ברק',
                        phone: '50411215',
                    },
                    {
                        tz: 207145244,
                        firstName: 'נעמי',
                        lastName: 'פישביין',
                        birthDate: '07/05/1998',
                        address: 'רשבם 22 בני ברק',
                        phone: '50411215',
                    },

                ],
                studentsFields: [
                    'ת.ז.',
                    'שם משפחה',
                    'שם פרטי',
                    'תאריך לידה',
                    'כתובת',
                    'טלפו'
                ]
            }
        }
    }
</script>

<style scoped>

</style>
