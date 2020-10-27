<template>
  <div class="q-pa-md">
    <q-page-container>
      <q-page padding>

        <q-page-sticky position="bottom-right" :offset="[18, 18]">
          <q-fab
            icon="add"
            direction="up"
            color="accent"
          >
            <q-fab-action @click="onDailyForm" type="button"  color="primary" icon="person_add"  />
            <q-fab-action @click="onPainForm" color="primary" icon="las la-dizzy" />
          </q-fab>
        </q-page-sticky>
      </q-page>
    </q-page-container>
  </div>
</template>

<script>
export default {
  name: 'BookAddBtnElement',

  methods: {
    onDailyForm () {
      this.$router.push('dailyForm')
    },
    onPainForm () {
      this.$router.push('painForm')
    }
  }
}
</script>
