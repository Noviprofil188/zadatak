<template>
    <q-page>
      <div class="q-pa-md q-gutter-sm">
        <q-banner inline-actions rounded class="bg-orange text-white">
          Ovo je dodani banner za Quasar.
  
          <template v-slot:action>
            <q-btn flat label="Klik" @click="onClick" />
            <q-btn flat label="Dismiss" @click="onDismiss" />
          </template>
        </q-banner>
      </div>
    </q-page>
  </template>
  
  <script>
  export default {
    name: 'UnosPage',
    methods: {
      onClick() {
        this.$q.notify({
          message: 'Gumb "Klik" je pritisnut!',
          color: 'green',
          position: 'top',
        });
      },
      onDismiss() {
        this.$q.notify({
          message: 'Banner je zatvoren.',
          color: 'red',
          position: 'top',
        });
      }
    }
  }
  </script>
