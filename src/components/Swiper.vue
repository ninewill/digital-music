<template>
  <div class="swiper-box">
    <div class="swiper-top">
      <div class="swiper-top-title">
        <div class="swiper-top-img">
          <img src="@/assets/images/pic/pic_05_APPEDU.svg" />
        </div>
        <p>流行音樂課程必學的四大理由</p>
      </div>
      <div class="swiper mySwiper2">
        <div class="swiper-wrapper swiper-flex">
          <div class="swiper-slide">
            <img src="@/assets/images/pic/pic_05-1_1x.png" />
          </div>
          <div class="swiper-slide">
            <img src="@/assets/images/pic/pic_05-2_1x.png" />
          </div>
          <div class="swiper-slide">
            <img src="@/assets/images/pic/pic_05-3_1x.png" />
          </div>
          <div class="swiper-slide">
            <img src="@/assets/images/pic/pic_05-4_1x.png" />
          </div>
        </div>
      </div>
    </div>

    <div thumbsSlider="" class="swiper mySwiper">
      <div class="swiper-wrapper swiper-item">
        <div class="swiper-slide swiper-list">
          <span class="slide-title">REASON 01</span>
          <img src="@/assets/images/pic/pic_05-5_1x.jpeg" />
          <div class="swiper-info">
            <div class="swiper-info-img">
              <img src="@/assets/images/pic/pic_05-9.svg" />
            </div>
            <span>授課一人一組配備， 熟悉每個工具的功能及特色</span>
          </div>
        </div>
        <div class="swiper-slide swiper-list">
          <span class="slide-title">REASON 02</span>
          <img src="@/assets/images/pic/pic_05-6_1x.jpeg" />
          <div class="swiper-info">
            <div class="swiper-info-img">
              <img src="@/assets/images/pic/pic_05-10.svg" />
            </div>
            <span>參訪知名產業公司， 了解專業設備環境</span>
          </div>
        </div>
        <div class="swiper-slide swiper-list">
          <span class="slide-title">REASON 03</span>
          <img src="@/assets/images/pic/pic_05-7_1x.jpeg" />
          <div class="swiper-info">
            <div class="swiper-info-img">
              <img src="@/assets/images/pic/pic_05-11.svg" />
            </div>
            <span>業界知名音樂人， 引薦投稿公司管道</span>
          </div>
        </div>
        <div class="swiper-slide swiper-list">
          <span class="slide-title">REASON 04</span>
          <img src="@/assets/images/pic/pic_05-8_1x.jpeg" />
          <div class="swiper-info">
            <div class="swiper-info-img">
              <img src="@/assets/images/pic/pic_05-12.svg" />
            </div>
            <span>全方位專業課程教學， 最高規格電腦教室</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  mounted() {
    var swiper = new Swiper('.mySwiper', {
      spaceBetween: 10,
      slidesPerView: 4,
      freeMode: true,
      watchSlidesProgress: true,
    });
    var swiper2 = new Swiper('.mySwiper2', {
      spaceBetween: 10,
      navigation: {
        nextEl: '.swiper-button-next',
        prevEl: '.swiper-button-prev',
      },
      thumbs: {
        swiper: swiper,
      },
    });
  },
};
</script>

<style lang="scss">
@import '@/assets/scss/mixin.scss';
@import '@/assets/scss/variables.scss';
@import '@/assets/scss/reset.scss';
@import '@/assets/scss/swiper.scss';

.swiper-wrapper {
  justify-content: space-between;

  @include min-width(768px) {
    margin-top: 3rem;
  }

  @include min-width(1025px) {
    margin-top: 0;
  }
}

.swiper-flex {
  @include min-width(1025px) {
  }
}

.swiper-item {
  flex-wrap: wrap;

  @include min-width(1025px) {
    flex-wrap: nowrap;
  }
}

.swiper-list {
  margin-bottom: 2rem;
  margin-right: 0 !important;

  @include min-width(1025px) {
    margin-right: 10px;
    margin-bottom: 0;
  }

  @include max-width(1025px) {
    width: 48% !important;
  }
}

.swiper-box {
  //position: relative;
  overflow: hidden;
  width: calc(100% - 40px);
  margin: 0 auto;
  margin-top: 2rem;

  @include min-width(768px) {
    width: calc(100% - 80px);
    margin-top: 5rem;
  }

  @include min-width(1025px) {
    width: 935px;
  }

  @include min-width(1440px) {
    width: 1200px;
  }

  @include min-width(1920px) {
    width: 1400px;
  }
}

.swiper-top {
  @include min-width(1025px) {
    display: flex;
  }
}

.swiper-top-title {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;

  @include min-width(1025px) {
    width: 30%;
  }

  .swiper-top-img {
    width: 40%;
    display: block;

    @include min-width(768px) {
      width: 30%;
    }

    @include min-width(1025px) {
      width: 100%;
    }

    > img {
      width: 100%;
    }
  }

  > p {
    width: 100%;
    font-weight: 700;
    font-size: 18px;
    line-height: 71px;
    text-align: center;
    background: linear-gradient(137.1deg, #fff176 14.56%, #00e0b8 85.34%);
    background-clip: text;
    color: transparent;

    @include min-width(768px) {
      margin-top: 1rem;
      font-size: 24px;
    }

    @include min-width(1025px) {
      font-size: 30px;
      line-height: 50px;
      text-align: left;
    }

    @include min-width(1440px) {
      font-size: 48px;
      line-height: 71px;
    }
  }
}

.swiper-info {
  margin-top: 1rem;

  @include min-width(768px) {
    margin-top: 2rem;
    padding: 0 2rem;
  }

  @include min-width(1025px) {
    padding: 0 1rem;
  }

  @include min-width(1440px) {
    padding: 0 3rem;
  }

  @include min-width(1920px) {
    padding: 0 5rem;
  }

  .swiper-info-img {
    width: 50%;
    margin: 0 auto;

    @include min-width(1025px) {
      width: 80%;
    }

    > img {
      width: 100%;
    }
  }

  > span {
    margin-top: 1rem;
    display: block;
    color: $color-white;
    line-height: 20px;
    font-weight: 400;
    font-size: 2vw;

    @include min-width(768px) {
      line-height: 28px;
    }

    @include min-width(1025px) {
      font-size: 16px;
      line-height: 23px;
    }
  }
}

.swiper-slide {
  text-align: center;
  font-size: 18px;
  background-size: cover;
  background-position: center;
  cursor: pointer;
}

.swiper-slide img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.slide-title {
  margin-bottom: 1rem;
  display: block;
  font-weight: 500;
  font-size: 18px;
  line-height: 30px;
  background: linear-gradient(137.1deg, #fff176 14.56%, #00e0b8 85.34%);
  background-clip: text;
  color: transparent;

  @include min-width(768px) {
    font-size: 26px;
  }
}

.swiper {
  width: 100%;
  height: 400px;
  margin-left: auto;
  margin-right: auto;

  @include min-width(768px) {
    height: 500px;
  }

  @include min-width(1025px) {
    height: 300px;
  }

  @include min-width(1440px) {
    height: 350px;
  }
}

.mySwiper2 {
  width: 90%;
  height: 80%;
  margin: 0 auto;
  overflow: hidden;
  position: relative;

  @include min-width(768px) {
    position: static;
  }

  @include min-width(1025px) {
    width: 60%;
    margin-right: 0;
    margin-left: auto;
  }

  &::after {
    content: '';
    display: block;
    position: absolute;
    bottom: 0;
    left: 0;
    z-index: 5;
    width: 100%;
    height: 2px;
    background-color: $color-primary-1;

    @include min-width(484px) {
      top: 99%;
      bottom: auto;
    }

    @include min-width(768px) {
      top: 42%;
    }

    @include min-width(1025px) {
      top: auto;
      bottom: 420px;
    }

    @include min-width(1280px) {
      bottom: 422px;
    }

    @include min-width(1440px) {
      bottom: 464px;
    }

    @include min-width(1920px) {
      bottom: 492px;
    }
  }
}

.mySwiper {
  height: 20%;
  box-sizing: border-box;
  padding-top: 50px;

  @include min-width(768px) {
    padding-bottom: 50px;
  }
}

.mySwiper .swiper-slide {
  width: 25%;
  height: 100%;
  opacity: 0.4;
}

.mySwiper .swiper-slide-thumb-active {
  opacity: 1;
}

.swiper-slide-thumb-active {
  > img {
    border: 2px solid transparent;
    border-image: linear-gradient(to bottom right, #fff176 0%, #00e0b8 100%);
    border-image-slice: 1;

    @include min-width(768px) {
      border: 5px solid transparent;
      border-image: linear-gradient(to bottom right, #fff176 0%, #00e0b8 100%);
      border-image-slice: 1;
    }

    @include min-width(1025px) {
      border: 2px solid transparent;
      border-image: linear-gradient(to bottom right, #fff176 0%, #00e0b8 100%);
      border-image-slice: 1;
    }

    @include min-width(1440px) {
      border: 5px solid transparent;
      border-image: linear-gradient(to bottom right, #fff176 0%, #00e0b8 100%);
      border-image-slice: 1;
    }
  }
}
</style>
