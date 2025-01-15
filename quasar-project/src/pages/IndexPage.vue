<template>
  <q-page class="flex flex-center">
    <img
      alt="Veleri logo"
      src="~assets/preuzmi.png"
      style="width: 200px; height: 200px"
    >
  </q-page>
  <div class="q-pa-md q-gutter-sm">
    <q-banner inline-actions rounded class="bg-orange text-white">
      Ovo je dodani banner za quasar.

      <template v-slot:action>
        <q-btn flat label="Turn ON Wifi" />
        <q-btn flat label="Dismiss" />
      </template>
    </q-banner>
  </div>
</template>
