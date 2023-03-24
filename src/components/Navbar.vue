<template>
  <!--header-->
  <header id="header">
    <div class="mainheader">
      <div class="side-left">
        <div class="index-info floatbtn">
          <a href="javascript:;" class="top-btn" title="TOP">
            <img src="@/assets/images/newpic/s1_logo.svg" alt="圖片" />
          </a>
        </div>
      </div>
      <div class="side-right">
        <div class="side-right-block">
          <div class="logo-btn">
            <a
              href="https://www.appedu.com.tw/"
              target="_blank"
              title="赫彩設計學院"
              >赫彩設計學院</a
            >
          </div>
          <!--<div class="menu-btn">
            <a href="javascript:;" title="menu">menu</a>
          </div>-->
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  setup() {
    return {};
  },
  mounted() {
    /*
     * ==========================================================================
     * TOP 按鈕
     * ==========================================================================
     */

    const $window = $(window);
    let scrollTop = $window.scrollTop();
    const $floatBtn = $('.floatbtn');
    const $topBtn = $floatBtn.find('.top-btn');

    $topBtn.on('click', function () {
      $('html, body').animate(
        {
          scrollTop: 0,
        },
        800,
        function () {
          // $('#u').trigger('focus');
          $('.firstGoTo-btn').trigger('focus');
        }
      );
      return false;
    });
  },
};
</script>

<style lang="scss" scoped>
@import '@/assets/scss/mixin.scss';
@import '@/assets/scss/variables.scss';
@import '@/assets/scss/reset.scss';

// * ==========================================================================
// * 共用
// * ==========================================================================

// * ==========================================================================
// * HEADER 區塊
// * ==========================================================================

#header {
  margin-top: 25px;
  width: 100%;
  display: flex;
  justify-content: center;
  position: fixed;
  z-index: 999;

  @include min-width(1025px) {
    margin-top: 50px;
  }
}

.mainheader {
  width: calc(100% - 40px);
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-direction: column;
  margin: 0 auto;
  transition: 0.2s;

  @include min-width(768px) {
    width: calc(100% - 80px);
  }

  @include min-width(1025px) {
    width: 935px;
    flex-direction: row;
  }

  @include min-width(1440px) {
    width: 1200px;
  }

  @include min-width(1920px) {
    width: 1400px;
  }
}

.index-info {
  display: none;

  @include min-width(768px) {
    display: block;
    margin-left: 0;
    margin-right: auto;
    font-weight: 400;
    font-size: 18px;
    color: $color-primary-1;
  }

  @include min-width(1025px) {
    font-size: 24px;
  }
}

.side-right {
  width: 100%;
  order: 0;

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
      position: relative;

      > a {
        width: 100%;
        height: 100%;
        display: block;
        position: absolute;
        top: 0px;
        left: 0px;
        background: url('@/assets/images/newbtn/s0_appedo_default.svg')
          no-repeat center/contain;
        @include hidetext;
        transition: 0.2s;

        @include min-width(1025px) {
          &:hover {
            background: url('@/assets/images/newbtn/s0_appedo_hover.svg')
              no-repeat center/contain;
          }
        }
      }
    }

    //.menu-btn {
    //  width: 103px;
    //  height: 38px;
    //  display: block;
    //  position: relative;

    //  @include min-width(1025px) {
    //    //margin-right: 0rem;
    //  }

    //  > a {
    //    width: 100%;
    //    height: 100%;
    //    display: block;
    //    position: absolute;
    //    top: 0px;
    //    left: 0px;
    //    background: url("@/assets/images/btn/btn_menu_default.svg") no-repeat
    //      center/contain;
    //    @include hidetext;
    //    transition: 0.2s;

    //    @include min-width(1025px) {
    //      &:hover {
    //        background: url("@/assets/images/btn/btn_menu_hover.svg") no-repeat
    //          center/contain;
    //      }
    //    }
    //  }

    //  &.close-btn {
    //    > a {
    //      background: url("@/assets/images/btn/btn-close.svg") no-repeat
    //        center/contain;
    //    }
    //  }
    //}
  }
}
</style>
