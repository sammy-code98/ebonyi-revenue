<template>
  <q-layout view="lHh Lpr lFf">
    <q-header class="bg-grey-12 text-dark">
      <q-toolbar>
        <q-btn
          flat
          dense
          round
          icon="menu"
          aria-label="Menu"
          @click="leftDrawerOpen = !leftDrawerOpen"
        />

        <q-space></q-space>
        <!-- <q-toolbar-title>
          Revenue
        </q-toolbar-title> -->
        <q-avatar>
          <img src="~assets/logo-1.png" />
        </q-avatar>
        <div class="text-capitalize q-ml-sm text-h6 text-grey text-weight-bold">
          ebsirs
        </div>

        <q-space></q-space>

        <q-tabs v-model="tab" shrink stretch>
          <q-tab name="home" label="Home" class="text-capitalize text-grey text-weight-bold" />
          <q-tab name="tax" label="Tax Information"  class="text-capitalize text-grey text-weight-bold"/>
          <q-tab name="news" label="News" class="text-capitalize text-grey text-weight-bold"/>
          <q-tab name="faq" label="FAQ" class="text-capitalize text-grey text-weight-bold" />
          <q-btn-dropdown dense unelevated no-caps color="positive" label="Etax">
            <q-list>
              <q-item clickable v-close-popup>
                <q-item-section>
                  <q-item-label>Calculate tax</q-item-label>
                </q-item-section>
                <q-item-section side>
                  <q-icon name="mdi-calculator-variant" color="positive" />
                </q-item-section>
              </q-item>
            </q-list>
          </q-btn-dropdown>
        </q-tabs>
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
export default {
  name: "MainLayout",
  data() {
    return {
      tab: ""
    };
  }
};
</script>
