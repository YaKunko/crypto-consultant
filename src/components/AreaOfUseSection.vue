<template>
  <div class="column items-center area-of-use-section">
    <div class="section-header">Area of Use</div>
    <img src="/images/logo.png" alt="Logo" class="logo" />

    <div class="lines-container">
      <div class="line line-left"></div>
      <div class="line line-middle"></div>
      <div class="line line-right"></div>
    </div>
    <div class="row boxes-container">
      <div class="col-4 box box-left">Token trading learning</div>
      <div class="col-4 box box-middle">Country and region crypto policy analysis</div>
      <div class="col-4 box box-right">Crypto tax consultation</div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'AreaOfUseSection',
})
</script>

<style lang="scss">
// .area-of-use-section {
//   padding: 0 5%;
//   @media (max-width: 768px) {
//     padding: 0 0.5rem;
//   }

//   .logo-container {
//     margin-bottom: 4rem;
//     .logo {
//       width: 120px;
//       height: 120px;
//     }
//   }

//   .use-cases-container {
//     display: flex;
//     justify-content: space-between;
//     width: 100%;
//     max-width: 1200px;
//     position: relative;

//     &::before {
//       content: '';
//       position: absolute;
//       top: -50px;
//       left: 10%;
//       right: 10%;
//       height: 2px;
//       background: #000;
//       opacity: 0.1;
//     }

//     .use-case {
//       flex: 1;
//       max-width: 300px;
//       text-align: center;

//       .text-box {
//         padding: 1.5rem;
//         font-size: 1.25rem;
//       }
//     }
//   }
// }
.area-of-use-section {
  width: 100%; // adjust as needed
  height: 100dvh; // adjust as needed
  margin: 0 auto; // center horizontally on page

  .section-header {
    font-size: 3rem;
    line-height: 3rem;
    font-weight: 500;
    letter-spacing: -0.06rem;
    color: #000;
  }

  .logo {
    margin-top: 5rem;
    height: 10rem;
  }
  .lines-container {
    position: relative;
    width: 100%;
    height: 23rem;

    .line {
      position: absolute;
      width: 2px;
      background-color: #ccc;
      transform-origin: top; // pivot rotation at the top
    }

    .line-left {
      top: 0; // start from below the logo
      left: 50%;
      height: 32.5rem;
      transform: translateX(-4.4375rem) rotate(45deg);
    }

    .line-middle {
      top: 1.75rem;
      left: 50%;
      height: 21.25rem;
      transform: translateX(-1px);
    }

    .line-right {
      top: 0;
      left: 50%;
      height: 32.5rem;
      transform: translateX(4.4375rem) rotate(-45deg);
    }
  }
  .boxes-container {
    width: 100%;
    .box {
      padding: 20px;
      text-align: center;
      font-size: 2rem;
      line-height: 2.5rem;
      letter-spacing: -0.06rem;
      font-weight: 400;
    }
  }
}
</style>
