<template>
  <!--footer-->
  <footer id="footer">
    <div class="footer-wrap">
      <div class="footer-left">
        <div class="footer-logo">
          <a
            href="https://www.appedu.com.tw/"
            target="_blank"
            title="赫綵設計學院"
            >赫綵設計學院</a
          >
        </div>
        <div class="footer-contact"></div>
        <ul class="footer-media">
          <li class="footer-media-icon fb">
            <a href="https://www.facebook.com/appedu/" target="_blank"
              >facebook</a
            >
          </li>
          <li class="footer-media-icon line">
            <a
              href="https://page.line.me/ksn8716p?openQrModal=true"
              target="_blank"
              >line</a
            >
          </li>
          <li class="footer-media-icon yt">
            <a
              href="https://www.youtube.com/user/AppeduDesignTraining"
              target="_blank"
              >youtube</a
            >
          </li>
          <li class="footer-media-icon ig">
            <a href="https://www.instagram.com/appedudesign/" target="_blank"
              >instagram</a
            >
          </li>
        </ul>
      </div>
      <div class="footer-right">
        <div class="footer-copyright">
          <span>Copyright ©Appedu. All rights reserved.</span>
          <span
            >赫綵電腦有限公司保有活動內容更改之權利，最新資訊以活動網站為主</span
          >
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/mixin.scss";
@import "@/assets/scss/variables.scss";
@import "@/assets/scss/reset.scss";


// * ==========================================================================
// * FOOTER 區塊
// * ==========================================================================

#footer {
  width: 100%;
  padding: 18px 20px;
  background-color: $color-primary-1;

  @include min-width(768px) {
    padding: 18px 20px;
  }

  @include min-width(1025px) {
    padding: 18px 60px;
  }

  @include min-width(1440px) {
    padding: 1.5rem 120px;
  }
}

.footer-wrap {
  width: 100%;
  margin: 0 auto;

  @include min-width(1025px) {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  @include min-width(1440px) {
    width: 1200px;
  }

  @include min-width(1920px) {
    width: 1400px;
  }
}

.footer-left {
  width: 100%;

  @include min-width(1025px) {
    display: flex;
    align-items: center;
    width: 60%;
  }
}

.footer-right {
  width: 80%;
  margin: 0 auto;

  @include min-width(1025px) {
    width: 40%;
  }
}

.footer-logo {
  width: 168px;
  height: 38px;
  display: block;
  position: relative;
  margin: 0 auto;

  @include min-width(1025px) {
    width: 187px;
    height: 40px;
    margin-left: 0px;
    margin-right: 1rem;
  }

  @include min-width(1440px) {
    margin-right: 2rem;
  }

  @include min-width(1920px) {
    margin-right: 3.5rem;
  }

  > a {
    width: 100%;
    height: 100%;
    display: block;
    color: $color-white;
    background: url("@/assets/images/icon/Logo_Normal.svg") no-repeat
      center/contain;
    @include hidetext;
    transition: 0.2s;
  }
}

.footer-contact {
  width: 210px;
  height: 34px;
  margin: 0 auto;
  margin-top: 35px;
  background: url("@/assets/images/icon/Tel.svg") no-repeat center/contain;

  @include min-width(1025px) {
    margin-top: 0;
    margin-left: 0;
    margin-right: 1rem;
  }

  @include min-width(1440px) {
    margin-right: 2rem;
  }

  @include min-width(1920px) {
    margin-right: 3.5rem;
  }
}

.footer-media {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 35px;

  @include min-width(1025px) {
    margin-top: 0;
    justify-content: space-between;
  }

  .footer-media-icon {
    width: 30px;
    height: 30px;
    margin-right: 14px;
    background-position: 50% 50%;
    background-repeat: no-repeat;
    transition: 0.2s;

    &:last-child {
      margin-right: 0;
    }

    > a {
      width: 100%;
      height: 100%;
      display: block;
      @include hidetext;
    }
  }
}

.fb {
  background: url("@/assets/images/icon/Facebook_Normal.svg");
}
.line {
  background: url("@/assets/images/icon/Line_Normal.svg");
}
.yt {
  background: url("@/assets/images/icon/Youtube_Normal.svg");
}
.ig {
  background: url("@/assets/images/icon/Instagram_Normal.svg");
}

.footer-copyright {
  margin-top: 35px;

  @include min-width(1025px) {
    margin-top: 0;
    margin-left: 4rem;
  }

  > span {
    line-height: 1.5;
    display: block;
    color: $color-white;
    font-size: 14px;
    text-align: center;

    &:first-child {
      margin-bottom: 0.5rem;
    }

    @include min-width(1025px) {
      font-size: 14px;
      text-align: left;

      &:first-child {
        margin-bottom: 0rem;
      }
    }
  }
}
</style>