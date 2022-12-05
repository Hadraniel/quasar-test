<style>
.tab-active {
  color: yellow;
}
</style>

<template>
  <q-layout view="lHh Lpr lff">
    <!--   ##################HEADER START########################    -->
    <q-header bordered class="bg-primary text-white">
      <q-toolbar>
        <q-btn dense flat round icon="menu" @click="toggleLeftDrawer" />

        <q-toolbar-title class="text-weight-light"> Dashboard </q-toolbar-title>
      </q-toolbar>
    </q-header>
    <!--   ##################HEADER END########################    -->

    <!--   ##################DRAWER START########################    -->
    <q-drawer
      class="bg-primary text-white"
      show-if-above
      v-model="leftDrawerOpen"
      side="left"
      :width="300"
    >
      <!-- drawer content -->
      <q-list>
        <q-item
          active-class="tab-active"
          to="/home"
          clickable
          v-ripple
          exact
          id="item1"
        >
          <q-item-section avatar>
            <q-icon name="fa-solid fa-house" />
          </q-item-section>

          <q-item-section class="text-h7 text-weight-bold">Home</q-item-section>
        </q-item>

        <q-item
          active-class="tab-active"
          to="/contact"
          clickable
          v-ripple
          exact
        >
          <q-item-section avatar>
            <q-icon name="help" />
          </q-item-section>

          <q-item-section class="text-h7 text-weight-bold"
            >Contact Us</q-item-section
          >
        </q-item>

        <q-item active-class="tab-active" to="/charts" clickable v-ripple exact>
          <q-item-section avatar>
            <q-icon name="insert_chart" />
          </q-item-section>

          <q-item-section class="text-h7 text-weight-bold"
            >Charts</q-item-section
          >
        </q-item>
      </q-list>
    </q-drawer>
    <!--   ##################DRAWER END########################    -->
    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
  <!--   ###############################################################    -->
</template>
<script>
import { ref } from "vue";

export default {
  setup() {
    const leftDrawerOpen = ref(false);

    return {
      leftDrawerOpen,
      toggleLeftDrawer() {
        leftDrawerOpen.value = !leftDrawerOpen.value;
      },
    };
  },
};
</script>
