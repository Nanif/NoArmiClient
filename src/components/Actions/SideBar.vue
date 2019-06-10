<template lang="html">

  <div id="parentx">

    <vs-button @click="active=!active" color="primary" type="filled">פעולות על הקבוצה</vs-button>
    <vs-sidebar position-right  parent="body" default-index="1"  color="primary" class="sidebarx" spacer v-model="active">

      <div class="header-sidebar" >

      </div >
      <vs-divider class="diving" position="right">
        הנפקת תעודת זהות
      </vs-divider>

      <vs-sidebar-item index="1"  position="right" dir="rtl" >
        קביעת תור
          </vs-sidebar-item>

      <vs-sidebar-item index="2" position="right" dir="rtl" >
        הונפק
      </vs-sidebar-item>

      <vs-divider class="diving" position="right">
        הצהרה
      </vs-divider>

      <vs-sidebar-item index="3"  position="right" dir="rtl" >
        תשלום
      </vs-sidebar-item>
      <vs-sidebar-item index="4" position="right" dir="rtl" >
        קביעת תור
      </vs-sidebar-item>
      <vs-sidebar-item index="5" position="right" dir="rtl" >
        חתימה
      </vs-sidebar-item>

      <vs-divider class="diving" position="right">
        שליחת תצהיר לצבא
      </vs-divider>

      <vs-sidebar-item index="6"  position="right" dir="rtl" >
        שליחה בדואר רשום
      </vs-sidebar-item>
      <vs-sidebar-item index="7" position="right" dir="rtl" >
קבלת אישור      </vs-sidebar-item>
      <vs-sidebar-item index="8" position="right" dir="rtl" >
        וידוא מול הצבא
      </vs-sidebar-item>
      <vs-sidebar-item index="9" position="right" dir="rtl" >
       סגירת תיק
      </vs-sidebar-item>

<!--      <div class="footer-sidebar" slot="footer">-->
<!--        <vs-button icon="reply" color="danger" type="flat">log out</vs-button>-->
<!--        <vs-button icon="settings" color="primary" type="border"></vs-button>-->
<!--      </div>-->

    </vs-sidebar>
  </div>

</template>

<script>
export default {
  data: () => ({
    active: false
  })
}
</script>

<style lang="scss" scoped>
  .header-sidebar {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    width: 100%;
  }

  .diving {
    font-size: large;
    font-weight: bold;
  }

    button {
      margin-left: 10px;
    }

  .footer-sidebar {
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 100%;

    button {
      border: 0px solid rgba(0, 0, 0, 0) !important;
      border-left: 1px solid rgba(0, 0, 0, .07) !important;
      border-radius: 0px !important;
    }
  }
</style>
