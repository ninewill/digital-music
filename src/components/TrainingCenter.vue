<template>
  <div>
    <div class="tc-top">
      <div class="tc-left">
        <div class="tc-l-img">
          <img src="@/assets/images/newpic/s5_pic.png" alt="圖片" />
        </div>
      </div>
      <div class="tc-right">
        <div class="tc-r-img">
          <img src="@/assets/images/newpic/s5_man.png" alt="圖片" />
        </div>
      </div>
    </div>
    <div class="tc-bottom"></div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import '@/assets/scss/mixin.scss';
@import '@/assets/scss/variables.scss';
@import '@/assets/scss/reset.scss';
@import '@/assets/scss/animate.scss';

.tc-top {
  display: flex;
  align-items: center;
  justify-content: space-between;

  .tc-left {
    width: 80%;

    @include min-width(768px) {
      width: 60%;
    }

    .tc-l-img {
      > img {
        width: 100%;
      }
    }
  }

  .tc-right {
    width: 28%;

    .tc-r-img {
      position: relative;

      @include min-width(1025px) {
        animation: peopleBounce 2.5s ease-in-out infinite;
      }

      > img {
        width: 100%;
      }

      &::after {
        @include min-width(1025px) {
          content: '';
          position: absolute;
          top: -100px;
          display: block;
          width: 150px;
          height: 170px;
          background: url('@/assets/images/newpic/s5_note.png') no-repeat;
          background-size: contain;
          background-position: 50% 50%;
          animation: musicBounce 2.2s ease-in-out infinite;
        }
      }
    }
  }
}
</style>
