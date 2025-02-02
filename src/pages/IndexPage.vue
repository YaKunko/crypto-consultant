<template>
  <q-page class="column flex-center">
    <MainSection />
    <AreaOfUseSection />
  </q-page>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import MainSection from 'src/components/MainSection.vue'
import AreaOfUseSection from 'src/components/AreaOfUseSection.vue'
export default defineComponent({
  name: 'IndexPage',

  components: {
    MainSection,
    AreaOfUseSection,
  },
})
</script>
<style lang="scss"></style>
