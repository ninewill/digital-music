<template>
  <div class="course-area">
    <div class="s-title s2-title">
      <div class="s2-title-left">
        <div class="s2-title-left-l">
          <img src="@/assets/images/newpic/s4_part2.png" alt="圖片" />
        </div>
        <div class="s2-title-left-r">
          <div class="h3">Nuendo高效進階聲音後製神器</div>
          <p>更高的聲音品質、更強的影音後製功能，搶先全台唯一認證中心！</p>
        </div>
      </div>
      <div class="s2-title-right">
        <img src="@/assets/images/newpic/s4_p2hour.png" alt="圖片" />
      </div>
    </div>
    <!--COURSE Swiper-->
    <div class="swiper-slid-part2">
      <!-- Swiper -->
      <div class="swiper mySwiper-part2 section-block">
        <div class="swiper-wrapper">
          <div class="swiper-slide">
            <img src="@/assets/images/newpic/s4_p2_01.png" alt="圖片" />
          </div>
          <div class="swiper-slide">
            <img src="@/assets/images/newpic/s4_p2_02.png" alt="圖片" />
          </div>
          <div class="swiper-slide">
            <img src="@/assets/images/newpic/s4_p2_03.png" alt="圖片" />
          </div>
          <div class="swiper-slide">
            <img src="@/assets/images/newpic/s4_p2_04.png" alt="圖片" />
          </div>
          <div class="swiper-slide">
            <img src="@/assets/images/newpic/s4_p2_05.png" alt="圖片" />
          </div>
          <div class="swiper-slide">
            <img src="@/assets/images/newpic/s4_p2_06.png" alt="圖片" />
          </div>
        </div>
        <div class="page-p">
          <img class="" src="@/assets/images/newpic/s4_PAGE.svg" alt="圖片" />
        </div>
        <div class="swiper-pagination swiper-pagination-swiper"></div>
      </div>
      <div class="swiper-button-next arrow-btn-next4"></div>
      <div class="swiper-button-prev arrow-btn-prev4"></div>
    </div>
    <div class="course-btn">
      <a class="cd-popup-trigger2" href="javascript:;">觀看完整課綱</a>
    </div>
    <CdPopup01 />
  </div>
</template>

<script>
import CdPopup01 from '@/components/CdPopup02.vue';

export default {
  components: {
    CdPopup01,
  },
  mounted() {
    var swiper5 = new Swiper('.swiper-slid-part2 .mySwiper-part2', {
      slidesPerView: 1,
      spaceBetween: 15,
      slidesPerGroup: 3,
      breakpoints: {
        310: {
          slidesPerView: 1,
        },
        768: {
          slidesPerView: 2,
        },
        1025: {
          slidesPerView: 3,
        },
        1440: {
          slidesPerView: 3,
        },
      },
      pagination: {
        el: '.mySwiper-part2 .swiper-pagination',
        clickable: true,
      },
      navigation: {
        nextEl: '.arrow-btn-next4',
        prevEl: '.arrow-btn-prev4',
      },
    });
  },
};
</script>

<style lang="scss" scoped>
@import '@/assets/scss/mixin.scss';
@import '@/assets/scss/variables.scss';
@import '@/assets/scss/reset.scss';
@import '@/assets/scss/swiper.scss';

.course-area {
  position: relative;
}

.s2-title {
  display: flex;
  align-items: center;
  justify-content: space-between;

  .s2-title-left {
    width: 60%;
    display: flex;

    .s2-title-left-l {
      width: 25%;

      > img {
        width: 100%;
      }
    }

    .s2-title-left-r {
      width: 70%;
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      justify-content: center;

      > img {
        width: 100%;
      }

      .h3 {
        font-weight: 700;
        font-size: 32px;
        line-height: 46px;
        color: $color-primary-1;
      }

      p {
        margin-top: 1rem;
        font-weight: 350;
        font-size: 20px;
        color: $color-white;
      }
    }
  }

  .s2-title-right {
    width: 30%;

    > img {
      width: 100%;
    }
  }
}

.mySwiper-part2 {
  overflow: hidden;

    img {
    width: 100% !important;
    height: auto;

    @include min-width(1440px) {
      width: auto !important;
      height: 100%;
    }
  }
}

.swiper-slid-part2 {
  padding: 20px;
  margin-top: 3rem;
  position: relative;
  display: flex;
  justify-content: center;
  z-index: 10;

  &::after {
    content: '';
    display: block;
    width: 95%;
    height: 300px;
    margin: 0 auto;
    border: 1px solid $color-primary-1;
    position: absolute;
    top: 100px;
  }

  @include min-width(1025px) {
    margin-top: 3rem;
    padding: 30px;
  }
}

.arrow-btn-next4,
.arrow-btn-prev4 {
  width: 50px;
  height: 50px;
  margin-top: -25px;
  background-size: contain;

  > img {
    width: 100%;
  }
}

.arrow-btn-next4 {
  right: 5%;
  background-image: url('@/assets/images/newbtn/s4_arrow_default.svg');

  @include min-width(1280px) {
    right: 3%;
  }
  @include min-width(1440px) {
    right: 3%;
  }
  @include min-width(1920px) {
    right: 0;
  }
}

.arrow-btn-prev4 {
  left: 5%;
  background-image: url('@/assets/images/newbtn/s4_arrow_default.svg');
  @include min-width(1280px) {
    left: 3%;
  }
  @include min-width(1440px) {
    left: 3%;
  }
  @include min-width(1920px) {
    left: 0;
  }
}

.swiper-slide {
  > img {
    width: auto;
    margin: 0 auto;
  }
}

//觀看完整課綱 按鈕
.course-btn {
  position: absolute;
  bottom: -35px;
  left: 50%;
  z-index: 10;
  margin-left: -143.04px;

  @include min-width(768px) {
    bottom: -80px;
    margin-left: -178.8px;
  }

  @include min-width(1440px) {
    margin-left: -137.5px;
  }

  > a {
    display: block;
    width: 286.08px;
    height: 69.76px;
    background: url('@/assets/images/newbtn/s4_view_default.svg') no-repeat
      center/contain;
    @include hidetext;
    transition: 0.2s;

    @include min-width(768px) {
      width: 357.6px;
      height: 87.2px;
    }

    @include min-width(1025px) {
      &:hover {
        background: url('@/assets/images/newbtn/s4_view_hover.svg') no-repeat
          center/contain;
      }
    }

    @include min-width(1440px) {
      width: 275px;
      height: 70px;
    }
  }
}
</style>
