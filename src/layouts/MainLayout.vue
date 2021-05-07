<template>
  <q-layout view="lHh Lpr lFf">
    <q-header class="bg-grey-12 text-dark">
      <q-toolbar>
        <q-avatar class="q-ml-md">
          <img src="~assets/logo-1.png" />
        </q-avatar>
        <div class="text-capitalize q-ml-sm text-h6 text-grey text-weight-bold">
          ebsirs
        </div>
        <q-space></q-space>
        <!-- menu for large screens -->
        <q-tabs v-model="tab" shrink stretch class="gt-sm">
          <q-tab
            name="home"
            label="Home"
            class="text-capitalize text-grey text-weight-bold"
          />
          <q-tab
            name="tax"
            label="Tax Information"
            class="text-capitalize text-grey text-weight-bold"
          />
          <q-tab
            name="news"
            label="News"
            class="text-capitalize text-grey text-weight-bold"
          />
          <q-tab
            name="faq"
            label="FAQ"
            class="text-capitalize text-grey text-weight-bold"
          />
          <q-btn-dropdown
            dense
            unelevated
            no-caps
            color="positive"
            label="Etax"
          >
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

        <!-- menu for small screens -->
        <div class="lt-md">
          <q-btn-dropdown
            dense
            unelevated
            no-caps
            color="positive"
            label="Etax"
          >
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
          <q-btn flat dense round icon="menu" aria-label="Menu">
            <q-menu
              fit
              transition-show="scale"
              transition-hide="scale"
              class="q-mt-xl"
            >
              <q-list style="min-width: 350px">
                <q-item clickable>
                  <q-item-section
                    class="text-center text-weight-regular text-subtitle1"
                    >Home</q-item-section
                  >
                </q-item>
                <q-separator inset />

                <q-item clickable>
                  <q-item-section
                    class="text-center text-weight-regular text-subtitle1"
                    >Tax Information</q-item-section
                  >
                </q-item>
                <q-separator inset />

                <q-item clickable>
                  <q-item-section
                    class="text-center text-weight-regular text-subtitle1"
                    >News</q-item-section
                  >
                </q-item>
                <q-separator inset />

                <q-item clickable>
                  <q-item-section
                    class="text-center text-weight-regular text-subtitle1"
                    >FAQ</q-item-section
                  >
                </q-item>
              </q-list>
            </q-menu>
          </q-btn>
        </div>
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
      tab: "",
      mobileData: true,
      bluetooth: false
    };
  }
};
</script>
