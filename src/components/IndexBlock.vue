<template>
  <div>
    <div class="idx-banner-m"></div>
    <video class="" autoplay muted loop>
      <source src="@/assets/images/video/Comp1.mp4" type="video/mp4" />
    </video>
    <div class="sonic-nav">
      <ul>
        <li>
          <a href="#1" class="sonic-btn">課程內容</a>
        </li>
        <li>
          <a href="#2" class="sonic-btn">薪資落點</a>
        </li>
        <li>
          <a href="#3" class="sonic-btn">課程優勢</a>
        </li>
        <li>
          <a href="#4" class="sonic-btn">學習環境</a>
        </li>
      </ul>
    </div>
    <div class="sonic-wrap">
      <div class="sonic">
        <img
          class="sonic-p"
          src="@/assets/images/newpic/s1_text.png"
          alt="圖片"
        />
        <img
          class="sonic-m"
          src="@/assets/images/mobile/s01_s1_text.png"
          alt="圖片"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  mounted() {
    $('.sonic-btn').click(function () {
      let target = this.hash,
        $target = $(target).offset().top;

      $('html, body').animate({ scrollTop: $target }), 1500;
    });
  },
};
</script>

<style lang="scss" scoped>
@import '@/assets/scss/mixin.scss';
@import '@/assets/scss/variables.scss';
@import '@/assets/scss/reset.scss';

.idx-banner-m {
  display: block;
  width: 100%;
  padding-bottom: 203.46%;
  background: url('@/assets/images/mobile/s1_Banner.jpg');
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
    //padding-top: 2rem;
    display: block;
  }
}

.sonic-nav {
  position: fixed;
  top: 120px;
  left: 5%;
  z-index: 100;

  @include min-width(484px) {
    left: 3%;
  }

  @include min-width(768px) {
    left: 4%;
  }

  @include min-width(960px) {
    left: 3%;
  }

  @include min-width(1025px) {
    left: 3%;
    top: 150px;
  }

  @include min-width(1280px) {
    left: 12%;
  }

  @include min-width(1440px) {
    left: 10%;
  }

  @include min-width(1650px) {
    left: 12%;
  }

  @include min-width(1920px) {
    left: 15%;
  }

  @include min-width(2260px) {
    left: 20%;
  }

  > ul {
    > li {
      margin-bottom: 2rem;

      > a {
        display: block;
        color: $color-white;
        font-size: 1rem;
        writing-mode: vertical-lr;

        @include min-width(1025px) {
          font-size: 1rem;
        }

        @include min-width(1280px) {
          font-size: 1.2rem;
        }
      }
    }
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
  width: 100%;

  @include min-width(1025px) {
    width: 60%;
  }

  .sonic-p {
    display: none;
    @include min-width(1025px) {
      display: block;
    }
  }

  .sonic-m {
    display: block;

    @include min-width(1025px) {
      display: none;
    }
  }

  > img {
    width: 100%;
    object-fit: cover;
  }
}
</style>
