<template>
  <!--header-->
  <header id="header">
    <div class="mainheader">
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
          <div class="menu-btn">
            <a href="javascript:;" title="menu">menu</a>
          </div>
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
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/mixin.scss";
@import "@/assets/scss/variables.scss";
@import "@/assets/scss/reset.scss";

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
  justify-content: flex-end;
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
        //margin-right: 0rem;
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
</style>