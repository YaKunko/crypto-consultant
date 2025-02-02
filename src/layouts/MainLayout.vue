<template>
  <q-layout class="column main-layout">
    <q-header>
      <q-toolbar class="row no-wrap justify-between items-center">
        <div class="row no-wrap flex-center header-logo">
          <img src="/images/logo.png" style="margin-right: 0.5rem; width: 2.375rem" />
          LCC
        </div>
        <div class="flex flex-center launch-bot-btn">
          Launch
          <img src="/icons/download.svg" style="margin-left: 0.5rem" />
        </div>
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
    <q-footer class="row flex-center">
      <div class="column footer-block">
        <div class="row no-wrap">
          <div class="col-6 row no-wrap items-center header-logo">
            <img src="/images/logo.png" style="margin-right: 0.5rem; width: 2.375rem" />
            LCC
          </div>
        </div>
        <div class="row justify-between" style="margin-top: 4.875rem">
          <div class="column" style="gap: 0.5rem">
            <router-link to="/privacy-policy">Privacy Policy</router-link>
            <router-link to="/terms">Terms of Use</router-link>
          </div>
          <div>Crypto Consult © 2025</div>
        </div>
      </div>
    </q-footer>
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
  max-width: 100%;
  .q-toolbar {
    padding: 0.875rem 5%;
    border-bottom: 1px solid rgba(0, 0, 0, 0.1);
    background-color: #fff;
    @media (max-width: 768px) {
      padding: 0.875rem 0.5rem;
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
  .q-footer {
    background: #fff;
    max-width: 100%;

    .footer-block {
      margin: 3rem 16.25rem;
      padding: 2.75rem 3rem;
      border-radius: 1.5rem;
      background: rgba(250, 250, 250, 1);
      min-width: 57.625rem;
      max-width: 100%;
      font-size: 0.875rem;
      font-weight: 400;
      line-height: 1rem;
      color: #000;
      @media (max-width: $breakpoint-sm-max) {
        border-radius: 0;
        min-width: 100%;
        width: 100%;
      }
      .footer-navigation {
        margin-top: 4.25rem;
        gap: 1rem;
        div {
          cursor: pointer;
        }
      }
      a {
        color: #000;
      }
    }
  }
  .header-logo {
    font-family: 'Kanit', sans-serif;
    font-size: 2rem;
    font-weight: 300;
    color: #000;
  }
}
</style>
