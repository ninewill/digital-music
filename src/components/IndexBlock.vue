<template>
  <div>
    <div class="idx-banner-m"></div>
    <video class="" autoplay muted loop>
      <source src="@/assets/images/video/FINAL.mp4" type="video/mp4" />
    </video>
    <div class="sonic-wrap">
      <div class="sonic">
        <img src="@/assets/images/newpic/s1_text.png" alt="圖片" />
      </div>
    </div>
  </div>
</template>

<script>
export default {

};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/mixin.scss";
@import "@/assets/scss/variables.scss";
@import "@/assets/scss/reset.scss";

.idx-banner-m {
  display: block;
  width: 100%;
  padding-bottom: 203.46%;
  background: url("@/assets/images/pic/mobile/pic_00_banner.png");
  background-position: 50% 50%;
  background-repeat: no-repeat;
  background-size: cover;

  @include min-width(768px) {
    display: none;
  }
}


video {
  display: none;

  @include min-width(768px) {
    width: 100%;
    height: 100%;
    padding-top: 2rem;
    display: block;
  }
}

.sonic-wrap {
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;

  .sonic-title {
    width: 50%;
    position: absolute;

    > img {
      width: 100%;
      height: 100%;
    }
  }
}

.sonic {
  display: none;

  @include min-width(768px) {
    width: 60%;
    display: block;
  }

  > img {
    width: 100%;
    object-fit: cover;
  }
}
</style>