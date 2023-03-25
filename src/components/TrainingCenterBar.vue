<template>
  <div class="tc-bar-wrap">
    <div class="tc-info">
      <div class="h3">Nuendo 全台唯一德國原廠授權認證教育中心</div>
      <p>
        2022年赫綵設計學院獨家搶先獲得
        德國Steinberg原廠認證ATC，接軌業界專業升級。
      </p>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import '@/assets/scss/mixin.scss';
@import '@/assets/scss/variables.scss';
@import '@/assets/scss/reset.scss';

.tc-bar-wrap {
  width: 70%;
  display: flex;
  justify-content: center;
  align-items: center;

  @include min-width(1025px) {
    width: 100%;
  }

  .tc-info {
    position: relative;

    @include min-width(1025px) {
      margin-left: -15%;
    }

    > .h3 {
      line-height: 1.5em;
      font-size: 1rem;
      color: $color-primary-1;

      @include min-width(768px) {
        font-size: 3vw;
      }

      @include min-width(1025px) {
        font-size: 2vw;
      }
    }
    > p {
      margin-top: 1rem;
      line-height: 1.5em;
      font-size: 0.8rem;
      color: $color-white;

      @include min-width(768px) {
        font-size: 1.8vw;
      }

      @include min-width(1025px) {
        font-size: 1.2vw;
      }
    }

    &::before {
      @include min-width(768px) {
        content: '';
        position: absolute;
        top: 0;
        display: block;
        background: url('@/assets/images/newpic/s5_star.png') no-repeat;
        background-size: contain;
        background-position: 50% 50%;
        width: 60px;
        height: 60px;
        left: -100px;
      }

      @include min-width(960px) {
        width: 70px;
        height: 70px;
      }

      @include min-width(1025px) {
        width: 90px;
        height: 90px;
      }
    }

    &::after {
      content: '';
      position: absolute;
      top: 50%;
      right: -108px;
      margin-top: -80px;
      display: block;
      width: 100px;
      height: 141px;
      background: url('@/assets/images/newpic/s5_license.jpg') no-repeat;
      background-size: contain;
      background-position: 50% 50%;

      @include min-width(768px) {
        width: 150px;
        height: 213px;
        right: -200px;
        margin-top: -110px;
      }

      @include min-width(960px) {
        width: 180px;
        height: 255px;
        right: -200px;
        margin-top: -130px;
      }

      @include min-width(1025px) {
        width: 215px;
        height: 305px;
        right: -300px;
        margin-top: -152.5px;
      }
    }
  }
}
</style>
