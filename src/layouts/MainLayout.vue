<template>
  <q-layout class="main-layout" view="lHh Lpr lFf">
    <q-header>
      <q-toolbar class="row no-wrap justify-between items-center">
        <div class="row no-wrap flex-center header-logo">
          <img src="/images/logo.png" style="margin-right: 0.5rem; width: 2.375rem" />
          LCC
        </div>
        <div class="flex flex-center launch-bot-btn">Launch</div>
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'MainLayout',

  components: {},

  data() {
    return {
      leftDrawerOpen: false,
    }
  },

  methods: {
    toggleLeftDrawer() {
      this.leftDrawerOpen = !this.leftDrawerOpen
    },
  },
})
</script>

<style lang="scss">
.main-layout {
  .q-toolbar {
    padding: 0.875rem 5%;
    border-bottom: 1px solid rgba(0, 0, 0, 0.1);
    background-color: #fff;
    @media (max-width: 768px) {
      padding: 0.875rem 0.5rem;
    }
    .header-logo {
      font-family: 'Kanit', sans-serif;
      font-size: 2rem;
      font-weight: 300;
      color: #000;
    }
    .launch-bot-btn {
      color: #fff;
      padding: 0.875rem 1.875rem;
      background-color: #000;
      border-radius: 0.625rem;
      font-size: 0.875rem;
      font-weight: 600;
      line-height: 1.25rem;
      height: 3rem;
      cursor: pointer;
    }
  }
}
</style>
