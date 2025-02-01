<template>
  <div class="row flex-center main-section">
    <div class="col-6 column main-section-content">
      <div class="main-section-content-title">Legal Crypto Consultant</div>
      <div class="main-section-content-description">
        Your AI consultant in the world of crypto regulation and taxation.
      </div>
      <div class="row no-wrap items-center main-section-content-buttons">
        <div class="flex flex-center external-link-btn">
          <a class="flex flex-center" style="padding: 0" href="https://x.com" target="_blank">
            <img src="/icons/twitter-icon.svg" alt="X logo" />
          </a>
        </div>
        <div class="flex flex-center external-link-btn">
          <a class="flex flex-center" href="https://dev.rivens.ai/" target="_blank">Rivens</a>
        </div>
      </div>
    </div>
    <div class="col main-section-content-image">
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
  padding: 0 5%;
  @media (max-width: 768px) {
    padding: 0 0.5rem;
  }
  .main-section-content {
    max-width: 100%;

    .main-section-content-title {
      max-width: 100%;
      font-size: 3rem;
      line-height: 3rem;
      font-weight: 500;
      letter-spacing: -0.06rem;
      color: #000;
    }
    .main-section-content-description {
      font-family: 'Kanit', sans-serif;
      margin-top: 1.5rem;
      font-size: 1.5rem;
      line-height: 2rem;
      font-weight: 500;
      color: rgba(0, 0, 0, 0.6);
      max-width: 80%;
    }
    .main-section-content-buttons {
      max-width: 100%;
      margin-top: 2rem;
      gap: 2rem;
      .external-link-btn {
        color: #fff;
        background-color: #000;
        border-radius: 0.625rem;
        font-size: 0.875rem;
        font-weight: 600;
        line-height: 1.25rem;
        height: 3.25rem;
        max-width: 40%;
        width: 14.5rem;
        a {
          width: 100%;
          height: 100%;
          padding: 0.875rem 1.875rem;
          color: #fff;
          text-decoration: none;
        }
      }
    }
  }
  .main-section-content-image {
    padding-left: 1rem;
  }
}
</style>
