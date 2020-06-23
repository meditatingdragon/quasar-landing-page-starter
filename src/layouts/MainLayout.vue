<template>
  <q-layout view="lHh Lpr lff">
    <q-header dark class="bg-green">
      <q-toolbar>
        <q-avatar>
          <img src="icons/favicon-32x32.png" />
        </q-avatar>
        <q-toolbar-title>
          Landing Page Templates
        </q-toolbar-title>
        <q-space />
        <q-btn flat to="/layout1">Layout 1</q-btn>
        <q-btn flat to="/layout2">Layout 2</q-btn>
      </q-toolbar>
    </q-header>
    <q-page-container>
      <router-view />
    </q-page-container>
    <Footer />
  </q-layout>
</template>

<script>
import Footer from "../components/Footer";

export default {
  name: "MainLayout",
  data() {
    return {
      leftDrawerOpen: false
    };
  },
  components: {
    Footer
  }
};
</script>
