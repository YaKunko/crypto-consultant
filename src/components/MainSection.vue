<template>
  <div class="row flex-center main-section">
    <div class="col-6 column main-section-content">
      <div class="main-section-content-title">Legal Crypto Consultant</div>
      <div class="main-section-content-description">
        Your AI consultant in the world of crypto regulation and taxation.
      </div>
    </div>
    <div class="col-6 main-section-content-image">
      <img
        src="/images/crypto-consult.png"
        alt="Main Section Image"
        style="max-width: 100%; width: 30rem"
      />
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'MainSection',

  data() {
    return {
      clickCount: 0,
    }
  },
})
</script>

<style lang="scss">
.main-section {
  .main-section-content {
    .main-section-content-title {
      font-size: 3rem;
      line-height: 3rem;
      font-weight: 500;
      letter-spacing: -0.06rem;
      color: #000;
    }
    .main-section-content-description {
      margin-top: 1.5rem;
      font-size: 1.5rem;
      line-height: 2rem;
      font-weight: 500;
      color: rgba(0, 0, 0, 0.6);
    }
  }
}
</style>
