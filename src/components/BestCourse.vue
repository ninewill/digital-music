<template>
  <div class="section4-1">
    <div class="s1-content-title-2">
      <div class="h3">三個月課程，讓你扎實踏入成音世界</div>
      <span class="s1-description">每次教學，我們都全力以赴</span>
    </div>
    <div class="iframe">
      <iframe
        src="https://www.youtube.com/embed/gz_t8COqFyw"
        title="YouTube video player"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
        allowfullscreen
      ></iframe>
    </div>
    <div class="curse-info">
      <div class="curse-info-left">
        <div class="curse-info-title">
          <h3 class="h3">學習事半功倍</h3>
          <span>業界音效師教你賦予影片靈魂的關鍵！</span>
        </div>
        <ul class="curse-info-item">
          <li>數位配樂</li>
          <li>音效設計</li>
          <li>混音實作</li>
          <li>錄音室實戰</li>
        </ul>
        <p>
          數位成音的範疇就是用聲音及音樂為影像加分，如果你對音效師的工作內容充滿好奇、熱忱，這裡提供全方位數位成音課程，重金禮聘業界音效師親自指導，讓學員學習配樂、音效、混音的完整製作流程，以及實際操作錄音設備，培養對影片音效的敏銳度和音樂創作力。
        </p>
      </div>
      <div class="curse-info-right">
        <div class="curse-img">
          <img src="@/assets/images/newpic/s9_environment.svg" alt="圖片" />
        </div>
        <!-- swiper -->
        <div class="swiper swiper-course">
          <div class="swiper-wrapper swiper-course-s">
            <div class="swiper-slide">
              <div class="main-img">
                <img src="@/assets/images/newpic/s9_e1.png" alt="圖片" />
              </div>
            </div>
            <div class="swiper-slide">
              <div class="main-img">
                <img src="@/assets/images/newpic/s9_e2.png" alt="圖片" />
              </div>
            </div>
            <div class="swiper-slide">
              <div class="main-img">
                <img src="@/assets/images/newpic/s9_e3.png" alt="圖片" />
              </div>
            </div>
            <div class="swiper-slide">
              <div class="main-img">
                <img src="@/assets/images/newpic/s9_e4.png" alt="圖片" />
              </div>
            </div>
          </div>
          <div class="swiper-pagination pagination-course"></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  mounted() {
    var swiper5 = new Swiper('.swiper-course', {
      pagination: {
        el: '.swiper-course .swiper-pagination',
        clickable: true,
      },
    });
  },
};
</script>

<style lang="scss" >
@import '@/assets/scss/mixin.scss';
@import '@/assets/scss/variables.scss';
@import '@/assets/scss/reset.scss';
@import '@/assets/scss/animate.scss';
@import '@/assets/scss/swiper.scss';

.section4-1 {
  width: 100%;
  height: 900px;
  position: absolute;
  margin-top: -65%;

  @include min-width(1025px) {
    margin-top: -75%;
  }

  @include min-width(1280px) {
    margin-top: -70%;
  }

  @include min-width(1400px) {
    margin-top: -65%;
  }

  @include min-width(1650px) {
    margin-top: -66%;
  }

  @include min-width(1920px) {
    margin-top: -70%;
  }

  @include min-width(2100px) {
    margin-top: -80%;
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

  .iframe {
    width: 100%;
    height: 56%;
    margin: 0 auto;
    margin-top: 5rem;

    @include min-width(1280px) {
      width: 80%;
    }

    @include min-width(1440px) {
      width: 80%;
      height: 66%;
    }

    > iframe {
      width: 100%;
      height: 100%;
    }
  }
}

.s1-content-title-2 {
  width: 870px;
  margin: 0 auto;
  position: relative;
  margin-top: 5rem;
  text-align: center;
  display: flex;
  flex-direction: column;

  &:before {
    content: '';
    position: absolute;
    top: -120px;
    left: -400px;
    width: 136px;
    height: 136px;
    display: block;
    background: url('@/assets/images/newpic/s9_bg_deco.png') no-repeat;
    background-size: contain;
    background-position: 50% 50%;

    @include min-width(1025px) {
      left: -150px;
    }

    @include min-width(1650px) {
      left: -400px;
    }
  }

  &::after {
    @include min-width(1025px) {
      content: '';
      position: absolute;
      top: 150px;
      width: 124px;
      height: 140px;
      display: block;
      background: url('@/assets/images/newpic/s9_note.png') no-repeat;
      background-size: contain;
      background-position: 50% 50%;
      right: -150px;
      animation: musicBounce 2.8s ease-in-out infinite;
    }

    @include min-width(1650px) {
      right: -350px;
    }
  }

  > .h3 {
    display: flex;
    justify-content: center;
    position: relative;
    padding: 2rem 3rem;
    display: block;
    border: 1px solid $color-primary-1;
    border-radius: 15px;
    font-weight: 700;
    font-size: 28px;
    color: $color-primary-1;

    &::before {
      content: '';
      display: block;
      position: absolute;
      top: -35px;
      left: 50%;
      margin-left: -131px;
      width: 262px;
      height: 48px;
      background: url('@/assets/images/newpic/s9_title.png') no-repeat;
      background-size: contain;
      background-position: 50% 50%;
    }
  }
  > .s1-description {
    margin-top: 1.5rem;
    position: relative;
    display: block;
    font-size: 24px;
    color: $color-white;

    &::after {
      content: '';
      display: block;
      margin-top: -8px;
      position: absolute;
      top: 50%;
      left: 180px;
      width: 90px;
      height: 16px;
      background: url('@/assets/images/newpic/s0_line.svg') no-repeat;
      background-size: contain;
      background-position: 50% 50%;
    }

    &:before {
      content: '';
      display: block;
      margin-top: -8px;
      position: absolute;
      top: 50%;
      right: 180px;
      width: 90px;
      height: 16px;
      background: url('@/assets/images/newpic/s0_line.svg') no-repeat;
      background-size: contain;
      background-position: 50% 50%;
      transform: scaleX(-1);
    }
  }
}

.curse-info {
  width: 80%;
  margin: 0 auto;
  padding: 3rem 0;
  padding-right: 50px;
  margin-top: 5rem;
  border-top: 1px dashed $color-primary-1;
  border-bottom: 1px dashed $color-primary-1;
  display: flex;
  justify-content: space-between;

  .curse-info-left {
    width: 45%;

    .curse-info-title {
      > .h3 {
        font-size: 36px;
        font-weight: 700;
        color: $color-primary-1;
      }

      > span {
        margin-top: 1.5rem;
        display: block;
        font-size: 22px;
        color: $color-white;
      }
    }

    .curse-info-item {
      margin-top: 1.5rem;
      padding: 0.5rem 1rem;
      display: flex;
      justify-content: center;
      border-top: 1px solid $color-primary-1;
      border-bottom: 1px solid $color-primary-1;

      > li {
        width: 23%;
        position: relative;
        display: flex;
        justify-content: center;
        align-items: center;
        color: $color-white;

        &::after {
          content: '';
          position: absolute;
          right: 0;
          display: block;
          width: 1px;
          height: 20px;
          background-color: $color-primary-1;
        }

        &:last-child {
          &::after {
            display: none;
          }
        }
      }
    }

    > p {
      font-size: 1rem;
      margin-top: 1rem;
      line-height: 2em;
      color: $color-white;
    }
  }
  .curse-info-right {
    width: 35%;
    display: flex;
    align-items: end;
    position: relative;

    &::after{
      content: "";
      display: block;
      position: absolute;
      right: -25px;
      bottom: 0;
      width: 1px;
      height: 200px;
      background-color: $color-primary-1;
    }

    .curse-img{
      margin-right: 1rem;

      >img{
        width: 100%;
      }
    }

    .swiper-course {
      // height: 100%;
      overflow: hidden;

      .swiper-course-s{

      }

      .pagination-course{
        top: 0;
        right: -40px;
        left: auto;
        display: flex;
        flex-direction: column;

        >span{
          margin-bottom: 20px;
        }
      }
    }
  }
}
</style>
