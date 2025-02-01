<template>
  <q-page class="column flex-center">
    <MainSection />
  </q-page>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import MainSection from 'src/components/MainSection.vue'

export default defineComponent({
  name: 'IndexPage',

  components: {
    MainSection,
  },
})
</script>
<style lang="scss"></style>
