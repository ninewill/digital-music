<template>
  <div class="section4-2">
    <div class="section-border"></div>
    <div class="section-block section-block1">
      <div class="s4-2-content-title-pc">
        <img src="@/assets/images/pic/pic_08_title.svg" alt="圖片" />
      </div>
      <div class="s4-2-content-title-mb">
        <img src="@/assets/images/pic/mobile/pic_08_title08.svg" alt="圖片" />
      </div>
      <div class="section-block-wrap">
        <div class="section-block-wrap-left">
          <div class="title-pc">
            <img src="@/assets/images/pic/pic_08-1_title.svg" alt="圖片" />
          </div>
          <div class="title-mb">
            <img
              src="@/assets/images/pic/mobile/pic_08_content.svg"
              alt="圖片"
            />
          </div>
          <span>音樂製作人｜作詞曲創作｜編曲創作｜ 專業歌手｜錄音混音</span>
          <p>
            音樂製作適合有著熱忱、好奇心、創新的你，愛唱歌、喜愛創作、後製混音、不限縮自我風格，零基礎的初學者72小時蛻變成為頂尖音樂製作人，掌握詞曲編錄混唱精髓，深入瞭解產業定位，準備好自己的武器，即能有所源源不絕案子。
          </p>
        </div>
        <div class="section-block-wrap-right">
          <video class="" autoplay muted controls>
            <source src="@/assets/images/video/Mike.mp4" type="video/mp4" />
          </video>
        </div>
      </div>
    </div>
    <div class="swiper-slid-w">
      <!-- Swiper -->
      <div class="swiper mySwiper1 section-block">
        <div class="swiper-wrapper">
          <div class="swiper-slide">
            <img src="@/assets/images/pic/pic_05-6_2x.jpeg" alt="圖片" />
          </div>
          <div class="swiper-slide">
            <img src="@/assets/images/pic/pic_08-3_2x.jpg" alt="圖片" />
          </div>
          <div class="swiper-slide">
            <img src="@/assets/images/pic/pic_08-4_2x.jpg" alt="圖片" />
          </div>
          <div class="swiper-slide">
            <img src="@/assets/images/pic/pic_08-5_2x.jpg" alt="圖片" />
          </div>
          <div class="swiper-slide">
            <img src="@/assets/images/pic/pic_08-6_2x.jpg" alt="圖片" />
          </div>
          <div class="swiper-slide">
            <img src="@/assets/images/pic/pic_08-7_2x.jpg" alt="圖片" />
          </div>
          <div class="swiper-slide">
            <img src="@/assets/images/pic/pic_08-8_2x.jpg" alt="圖片" />
          </div>
          <div class="swiper-slide">
            <img src="@/assets/images/pic/pic_08-9_2x.jpg" alt="圖片" />
          </div>
        </div>
      </div>
      <div class="swiper-button-next arrow-btn arrow-btn-next"></div>
      <div class="swiper-button-prev arrow-btn arrow-btn-prev"></div>
    </div>
    <div class="section-block section-block-2">
      <div class="section-block-title">
        <img src="@/assets/images/pic/pic_09.svg" alt="圖片" />
      </div>
      <div class="section-block-info">
        <p>將興趣轉為商機，再多一步就能有所改變</p>
        <span>從零基礎到進階，業師絕不吝傳授獨家技法！</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  mounted() {
    var swiper4 = new Swiper(".mySwiper1", {
      slidesPerView: 4,
      spaceBetween: 15,
      slidesPerGroup: 4,
      breakpoints: {
        310: {
          slidesPerView: 1,
          slidesPerGroup: 1,
        },
        1025: {
          slidesPerView: 3,
          slidesPerGroup: 3,
        },
        1440: {
          slidesPerView: 4,
          slidesPerGroup: 4,
        },
      },
      navigation: {
        nextEl: ".arrow-btn-next",
        prevEl: ".arrow-btn-prev",
      },
    });
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/mixin.scss";
@import "@/assets/scss/variables.scss";
@import "@/assets/scss/reset.scss";
@import "@/assets/scss/swiper.scss";
.section-block {
  width: calc(100% - 40px);
  margin: 0 auto;
  position: relative;
  @include min-width(525px) {
    width: calc(100% - 60px);
  }
  @include min-width(768px) {
    width: calc(100% - 80px);
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
  &:first-child {
    margin-top: 0;
  }
  &.section-block1 {

    @include min-width(1025px) {
			padding-top: 4rem;
      height: 500px;
    }
    @include min-width(1440px) {
      height: 600px;
    }
    @include min-width(1920px) {
      height: 650px;
    }
  }
  &.section-block-2 {
    padding: 5rem 1rem;

    @include min-width(1025px) {
        padding: 5rem;
    }
  }
  > h1 {
    font-size: 80px;
    color: $color-white;
  }
}

.section4-2 {
  margin-top: 2rem; //display: flex;
  //justify-content: center;
  position: relative;

	@include min-width(768px) {
		margin-top: 12rem;
	}



  .section-border {
    @include min-width(1025px) {
      position: absolute;
      left: 0;
      width: 70%;
      height: 700px;
      border-top: 1px solid $color-primary-1;
      border-right: 1px solid $color-primary-1;
    }
  }
}

.s4-2-content-title-pc {
  display: none;
  @include min-width(1025px) {
    display: block;
    width: 50%;
    position: absolute;
    margin-left: 0;
    margin-right: auto;
    margin-top: -145px;
  }
  @include min-width(1440px) {
    margin-top: -170px;
  }
  > img {
    width: 100%;
  }
}

.s4-2-content-title-mb {
  display: block;
  width: 88%;
	top: -25%;
	right: 0;
	left: 0;
	bottom: 0;
	margin: 0 auto;
  margin-right: auto;

	@include min-width(768px) {
		width: 50%;
		margin-left: 25%;
		position: absolute;
		top: -18%;
	}


  @include min-width(1025px) {
    display: none;
  }
  > img {
    width: 100%;
  }
}

.section-block-wrap {
  width: 100%;
  @include min-width(1025px) {
    display: flex;
    justify-content: space-between;
  }
  .section-block-wrap-left {
    width: 100%;
    margin-top: 0rem;

    @include min-width(1025px) {
      width: 35%;
      margin-left: 3rem;
    }
    @include min-width(1440px) {
      width: 28%;
      margin-top: 8rem;
      margin-left: 5rem;
    }
    @include min-width(1920px) {
      width: 24%;
    }
    .title-pc {
      width: 50%;
      display: none;

      @include min-width(1025px) {
        display: block;
      }

      > img {
        width: 100%;
      }
    }
    .title-mb {
      width: 80%;
      margin: 0 auto;
			margin-top: 2rem;
      display: block;

			@include min-width(768px) {
				width: 50%;
				margin-top: 0;
			}

      @include min-width(1025px) {
        display: none;
      }

      > img {
        width: 100%;
      }
    }
    > span {
      padding: 0 2rem;
      margin-top: 2rem;
      display: block;
      line-height: 30px;
      font-size: 16px;
      background: linear-gradient(137.1deg, #fff176 14.56%, #00e0b8 85.34%);
      background-clip: text;
      color: transparent;
      text-align: center;

			@include min-width(768px) {
				padding: 0 4rem;
				font-size: 18px;
			}


      @include min-width(1025px) {
        padding: 0;
        text-align: left;
      }
    }
    > p {
      margin-top: 2rem;
      line-height: 30px;
      color: $color-white;
			font-size: 14px;

			@include min-width(768px) {
        font-size: 16px;
      }
    }
  }
  .section-block-wrap-right {
    width: 100%;
    @include min-width(1025px) {
      width: 57%;
    }
    > video {
      width: 100%;
      height: 100%;
    }
  }
}

.mySwiper1 {
  overflow: hidden;
}

.swiper-slid-w {
  padding: 20px;
  margin-top: 3rem;
  position: relative;
  z-index: 10;
  background: linear-gradient(137.1deg, #fff176 14.56%, #00e0b8 85.34%);
  overflow: hidden;
  @include min-width(1025px) {
    margin-top: 1rem;
    padding: 30px;
  }
}

.arrow-btn {
  margin-top: -25px;
}

.arrow-btn-next {
  right: 5%;
  background-image: url("@/assets/images/icon/pic_08_arrow.svg");
  @include min-width(1280px) {
    right: 3%;
  }
  @include min-width(1440px) {
    right: 3%;
  }
  @include min-width(1920px) {
    right: 5%;
  }
}

.arrow-btn-prev {
  left: 5%;
  background-image: url("@/assets/images/icon/pic_08_arrow.svg");
  @include min-width(1280px) {
    left: 3%;
  }
  @include min-width(1440px) {
    left: 3%;
  }
  @include min-width(1920px) {
    left: 5%;
  }
}

.section-block-title {
  display: flex;
  justify-content: center;

  > img {
    width: 100%;
  }
}

.section-block-info {
  margin-top: 1rem;

  > p {
    margin-bottom: 0px;
    line-height: 50px;
    font-weight: 700;
    font-size: 16px;
    background: linear-gradient(137.1deg, #fff176 14.56%, #00e0b8 85.34%);
    background-clip: text;
    color: transparent;
    text-align: center;

    @include min-width(768px) {
      margin-bottom: 1rem;
      font-size: 18px;
    }

    @include min-width(1025px) {
      font-size: 30px;
    }
  }
  > span {
    display: block;
    font-weight: 400;
    font-size: 14px;
    color: $color-white;
    text-align: center;

    @include min-width(768px) {
      font-size: 16px;
    }

    @include min-width(1025px) {
      font-size: 20px;
    }
  }
}
</style>