<template>
  <!--menu-->
  <div class="menu-page">
    <!--menu header-->
    <div class="menu-header">
      <div class="menu-header-m">
        <div class="side-right">
          <div class="side-right-block">
            <div class="menu-btn close-btn">
              <a href="javascript:;" title="menu">menu</a>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="menu-page-content">
      <div class="menu-page-left">
        <div class="menu-page-left__bg">
          <img src="@/assets/images/pic/pic_00_photo.jpeg" alt="圖片" />
        </div>
      </div>
      <div class="menu-page-right">
        <div class="mic-icon">
          <img src="@/assets/images/pic/sticker.svg" alt="圖片" />
        </div>
        <div class="menu-title">
          <img src="@/assets/images/pic/pic_00_menutitle.svg" alt="圖片" />
        </div>
        <div class="menu-inner">
          <ol>
            <li class="menu-inner-list1">
              <a class="c-link" href="#1">
                <span>01</span>
                <div class="c-text">
                  <p>零基礎也能上手！</p>
                  <small>新手也能開始的音樂製作養成班</small>
                </div>
              </a>
            </li>
            <li class="menu-inner-list2">
              <a class="c-link" href="#2">
                <span>02</span>
                <div class="c-text">
                  <p>音樂製作養成首選！</p>
                  <small>最值得信賴的教學流程與豐富師資</small>
                </div>
              </a>
            </li>
            <li class="menu-inner-list3">
              <a class="c-link" href="#3">
                <span>03</span>
                <div class="c-text">
                  <p>眼見為憑，百聞不如一見！</p>
                  <small>最優質的學習環境＆學員見證分享</small>
                </div>
              </a>
            </li>
          </ol>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  mounted() {},
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/mixin.scss";
@import "@/assets/scss/variables.scss";
@import "@/assets/scss/reset.scss";

// * ==========================================================================
// * MENU 區塊
// * ==========================================================================

.menu-page {
  width: 100%;
  height: 100%;
  background-color: $color-primary-1;
  position: fixed;
  z-index: 1000;
}

.menu-header {
  margin-top: 25px;
  width: 100%;
  display: flex;
  justify-content: center;

  @include min-width(1025px) {
    margin-top: 50px;
  }
}

.menu-header-m {
  width: calc(100% - 40px);
  display: flex;
  justify-content: flex-end;
  align-items: center;
  margin: 0 auto;
  transition: 0.2s;

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
}

.side-right {
  width: auto;

  @include min-width(1025px) {
    width: auto;
  }

  .side-right-block {
    width: 100%;
    display: flex;
    justify-content: space-between;

    @include min-width(1025px) {
      width: auto;
    }

    .logo-btn {
      width: 167px;
      height: 38px;
      display: block;
      margin-right: 1rem;
      position: relative;

      > a {
        width: 100%;
        height: 100%;
        display: block;
        position: absolute;
        top: 0px;
        left: 0px;
        background: url("@/assets/images/btn/btn_appedu_default.svg") no-repeat
          center/contain;
        @include hidetext;
        transition: 0.2s;

        @include min-width(1025px) {
          &:hover {
            background: url("@/assets/images/btn/btn_appedu_hover.svg")
              no-repeat center/contain;
          }
        }
      }
    }

    .menu-btn {
      width: 103px;
      height: 38px;
      display: block;
      position: relative;

      @include min-width(1025px) {
        //margin-right: 2.5rem;
      }

      > a {
        width: 100%;
        height: 100%;
        display: block;
        position: absolute;
        top: 0px;
        left: 0px;
        background: url("@/assets/images/btn/btn_menu_default.svg") no-repeat
          center/contain;
        @include hidetext;
        transition: 0.2s;

        @include min-width(1025px) {
          &:hover {
            background: url("@/assets/images/btn/btn_menu_hover.svg") no-repeat
              center/contain;
          }
        }
      }

      &.close-btn {
        > a {
          background: url("@/assets/images/btn/btn-close.svg") no-repeat
            center/contain;
        }
      }
    }
  }
}

.menu-page-content {
  width: calc(100% - 40px);
  height: calc(100% - 100px);
  margin: 0 auto;
  overflow-y: auto;
  display: flex;
  justify-content: space-between;

  @include min-width(480px) {
    width: calc(100% - 120px);
  }

  @include min-width(768px) {
    width: 100%;
  }
}

.menu-page-left {
  display: none;

  @include min-width(768px) {
    width: 43%;
    display: block;
  }

  @include min-width(1025px) {
    width: 43%;
  }

  @include min-width(1280px) {
    width: 40%;
  }

  .menu-page-left__bg {
    width: 38%;
    height: 88vh;
    overflow: hidden;
    position: fixed;
    top: 0;
    left: 0;
    border-radius: 0 0 8rem 0;

    @include min-width(1025px) {
      width: 43%;
    }

    @include min-width(1280px) {
      width: 38%;
    }

    > img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
  }
}

.menu-page-right {
  width: 100%;
  height: 100%;
  overflow-y: auto;
  margin: 0 auto;
  margin-top: 2rem;

  @include min-width(768px) {
    width: 55%;
    margin-left: auto;
    margin-right: 2%;
  }

  @include min-width(1025px) {
    width: 43%;
    height: auto;
    margin-right: 8%;
  }

  @include min-width(1280px) {
    width: 35%;
    margin-right: 20%;
  }

  @include min-width(1440px) {
    width: 30%;
    margin-right: 25%;
  }

  .mic-icon {
    width: 20%;

    > img {
      width: 100%;
    }

    @include min-width(768px) {
      width: 30%;
    }

    @include min-width(1025px) {
      width: 25%;
    }

    @include min-width(1440px) {
      width: 35%;
    }

    @include min-width(1920px) {
      width: 25%;
    }
  }

  .menu-title {
    margin-top: 2rem;

    > img {
      width: 100%;
    }
  }

  .menu-inner {
    margin-top: 30px;

    .c-link {
      display: flex;
      align-items: flex-start;
      padding: 1rem 0;
      position: relative;
      border-bottom: 1px dashed $color-white;

      @include min-width(1440px) {
        padding: 2rem 0;
      }

      &:after {
        content: "";
        width: 1.474rem;
        height: 1.474rem;
        position: absolute;
        top: 0;
        bottom: 0;
        right: 2.2rem;
        margin: auto;
        background: url("@/assets/images/pic/pic_00_arrow.svg") no-repeat
          center/contain;
      }

      > span {
        margin-right: 35px;
        display: block;
        font-weight: 400;
        font-size: 1rem;
        color: $color-white;
      }

      .c-text {
        > p {
          margin-bottom: 0;
          font-weight: 700;
          font-size: 18px;
          color: $color-white;

          @include min-width(768px) {
            margin-bottom: 1rem;
            font-size: 20px;
          }

          @include min-width(1440px) {
            font-size: 24px;
          }
        }

        > small {
          font-weight: 400;
          font-size: 14px;
          color: $color-white;
          opacity: 0.7;

          @include min-width(768px) {
            font-size: 18px;
          }
        }
      }
    }
  }
}
</style>