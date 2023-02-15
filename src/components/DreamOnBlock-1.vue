<template>
  <div class="section4-1">
    <div class="s4-content-title">
      <img src="@/assets/images/pic/pic_08_slogan.svg" alt="圖片" />
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/mixin.scss";
@import "@/assets/scss/variables.scss";
@import "@/assets/scss/reset.scss";

.section4-1 {
  margin-top: 3rem;

  @include min-width(1025px) {
    margin-top: 7rem;
  }

  .s4-content-title {
    width: 100%;
    margin: 0 auto;

    @include min-width(1025px) {
      width: 70%;
    }

    > img {
      width: 100%;
    }
  }
}
</style>