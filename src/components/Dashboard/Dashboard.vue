<template>
    <div>
        <!--        <font-awesome-icon icon="coffee"/>-->

        <table class="table table-responsive-md table-fixed table-bordered table-striped" dir="rtl" id="tableFiles">
            <thead>
            <tr>
                <th :key="i" v-for="(field, i) in studentsFields"> {{ field }}</th>
            </tr>
            </thead>

            <tbody>
            <tr :key="idx" v-for="(student, idx) in studentsList[idx].list">
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
  data: function () {
    return {
      studentsList: [
        {
          name: 'חורף פ',
          list: [
            {
              tz: 207145244,
              firstName: 'נעמי',
              lastName: 'פישביין',
              birthDate: '07/05/1998',
              address: 'רשבם 22 בני ברק',
              phone: '50411215'
            },

            {
              tz: 207145244,
              firstName: 'נעמי',
              lastName: 'פישביין',
              birthDate: '07/05/1998',
              address: 'רשבם 22 בני ברק',
              phone: '50411215'
            },
            {
              tz: 207145244,
              firstName: 'נעמי',
              lastName: 'פישביין',
              birthDate: '07/05/1998',
              address: 'רשבם 22 בני ברק',
              phone: '50411215'
            },
            {
              tz: 207145244,
              firstName: 'נעמי',
              lastName: 'פישביין',
              birthDate: '07/05/1998',
              address: 'רשבם 22 בני ברק',
              phone: '50411215'
            },
            {
              tz: 207145244,
              firstName: 'נעמי',
              lastName: 'פישביין',
              birthDate: '07/05/1998',
              address: 'רשבם 22 בני ברק',
              phone: '50411215'
            },
            {
              tz: 207145244,
              firstName: 'נעמי',
              lastName: 'פישביין',
              birthDate: '07/05/1998',
              address: 'רשבם 22 בני ברק',
              phone: '50411215'
            }
          ]
        },
        {
          name: 'קיץ פ',
          list: [
            {
              tz: 207145244,
              firstName: 'יהודית',
              lastName: 'קובר',
              birthDate: '07/05/1998',
              address: 'רשבם 15 בני ברק',
              phone: '0504785412'
            },

            {
              tz: 207145244,
              firstName: 'יהודית',
              lastName: 'קובר',
              birthDate: '07/05/1998',
              address: 'רשבם 15 בני ברק',
              phone: '0504785412'
            },
            {
              tz: 207145244,
              firstName: 'יהודית',
              lastName: 'קובר',
              birthDate: '07/05/1998',
              address: 'רשבם 15 בני ברק',
              phone: '0504785412'
            },
            {
              tz: 207145244,
              firstName: 'יהודית',
              lastName: 'קובר',
              birthDate: '07/05/1998',
              address: 'רשבם 15 בני ברק',
              phone: '0504785412'
            },
            {
              tz: 207145244,
              firstName: 'יהודית',
              lastName: 'קובר',
              birthDate: '07/05/1998',
              address: 'רשבם 15 בני ברק',
              phone: '0504785412'
            },
            {
              tz: 207145244,
              firstName: 'יהודית',
              lastName: 'קובר',
              birthDate: '07/05/1998',
              address: 'רשבם 15 בני ברק',
              phone: '0504785412'
            }
          ]
        },
        {
          name: 'סתו פ',
          list: [
            {
              tz: 207145244,
              firstName: 'אסתר',
              lastName: 'יצחקוב',
              birthDate: '07/05/1998',
              address: 'וילקומירר 12 בני ברק',
              phone: '0548488994'
            },

            {
              tz: 207145244,
              firstName: 'אסתר',
              lastName: 'יצחקוב',
              birthDate: '07/05/1998',
              address: 'וילקומירר 12 בני ברק',
              phone: '0548488994'
            },
            {
              tz: 207145244,
              firstName: 'אסתר',
              lastName: 'יצחקוב',
              birthDate: '07/05/1998',
              address: 'וילקומירר 12 בני ברק',
              phone: '0548488994'
            },
            {
              tz: 207145244,
              firstName: 'אסתר',
              lastName: 'יצחקוב',
              birthDate: '07/05/1998',
              address: 'וילקומירר 12 בני ברק',
              phone: '0548488994'
            },
            {
              tz: 207145244,
              firstName: 'אסתר',
              lastName: 'יצחקוב',
              birthDate: '07/05/1998',
              address: {
                tz: 207145244,
                firstName: 'אסתר',
                lastName: 'יצחקוב',
                birthDate: '07/05/1998',
                address: 'וילקומירר 12 בני ברק',
                phone: '0548488994'
              }
            }
          ]
        },
        {
          name: 'אביב פ',
          list: [
            {
              tz: 207145244,
              firstName: 'מלכה',
              lastName: 'ברוק',
              birthDate: '07/05/1998',
              address: 'מצליח 10 בני ברק',
              phone: '0527603743'
            },

            {
              tz: 207145244,
              firstName: 'מלכה',
              lastName: 'ברוק',
              birthDate: '07/05/1998',
              address: 'מצליח 10 בני ברק',
              phone: '0527603743'
            },
            {
              tz: 207145244,
              firstName: 'מלכה',
              lastName: 'ברוק',
              birthDate: '07/05/1998',
              address: 'מצליח 10 בני ברק',
              phone: '0527603743'
            },
            {
              tz: 207145244,
              firstName: 'מלכה',
              lastName: 'ברוק',
              birthDate: '07/05/1998',
              address: 'מצליח 10 בני ברק',
              phone: '0527603743'
            },
            {
              tz: 207145244,
              firstName: 'מלכה',
              lastName: 'ברוק',
              birthDate: '07/05/1998',
              address: 'מצליח 10 בני ברק',
              phone: '0527603743'
            },
            {
              tz: 207145244,
              firstName: 'מלכה',
              lastName: 'ברוק',
              birthDate: '07/05/1998',
              address: 'מצליח 10 בני ברק',
              phone: '0527603743'
            },
            {
              tz: 207145244,
              firstName: 'מלכה',
              lastName: 'ברוק',
              birthDate: '07/05/1998',
              address: 'מצליח 10 בני ברק',
              phone: '0527603743'
            }
          ]
        }
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
