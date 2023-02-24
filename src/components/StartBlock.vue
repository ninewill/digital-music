<template>
  <div>
    <div class="s-title s1-title">
      <h2 class="h2">START</h2>
    </div>
    <div class="s-content s1-content">
      <!--start1-->
      <div class="s1-content-title-1">
        <div class="h3">
          為影像賦能的幕後推手——音效設計師、音訊工程師、配音員
        </div>
        <span class="s1-description"
          >完整系統化課程規劃，學習不再是當無頭蒼蠅</span
        >
      </div>
      <ul class="s1-item-wrap">
        <li>
          <div class="s1-img-1">
            <img
              src="@/assets/images/newpic/s2_learner01_default.png"
              alt="圖片"
            />
          </div>
          <div class="s1-img-2">
            <img
              src="@/assets/images/newpic/s2_learner01_hover.png"
              alt="圖片"
            />
          </div>
          <div class="h3">輔助影像學習者</div>
          <p class="s1-info">
            動畫師、遊戲設計師、影視特效師、配音員、擬音師、剪輯師
          </p>
        </li>
        <li>
          <div class="s1-img-1">
            <img
              src="@/assets/images/newpic/s2_learner02_default.png"
              alt="圖片"
            />
          </div>
          <div class="s1-img-2">
            <img
              src="@/assets/images/newpic/s2_learner02_hover.png"
              alt="圖片"
            />
          </div>
          <div class="h3">精進成音知識技術者</div>
          <p class="s1-info">系統化整合業界技術需求， 熟悉軟硬體操作模式</p>
        </li>
        <li>
          <div class="s1-img-1">
            <img
              src="@/assets/images/newpic/s2_learner03_default.png"
              alt="圖片"
            />
          </div>
          <div class="s1-img-2">
            <img
              src="@/assets/images/newpic/s2_learner03_hover.png"
              alt="圖片"
            />
          </div>
          <div class="h3">獨立接案專案管理者</div>
          <p class="s1-info">業界標準流程、接案報價 擬定合約、專案時程安排</p>
        </li>
      </ul>
      <!--start2-->
      <div class="s1-content-title-2">
        <div class="h3">全方位引領最快捷徑，培養業界爭搶人才</div>
        <span class="s1-description"
          >星耀級別配音、成音講師帶你階段性傳授業界技能</span
        >
      </div>
      <ul class="s1-item-2-wrap">
        <li>
          <div class="s1-img-1">
            <img src="@/assets/images/newpic/s3_card1_default.svg" alt="圖片" />
          </div>
          <div class="s1-img-2">
            <img src="@/assets/images/newpic/s3_card1_hover.svg" alt="圖片" />
          </div>
        </li>
        <li>
          <div class="s1-img-1">
            <img src="@/assets/images/newpic/s3_card2_default.svg" alt="圖片" />
          </div>
          <div class="s1-img-2">
            <img src="@/assets/images/newpic/s3_card2_hover.svg" alt="圖片" />
          </div>
        </li>
        <li>
          <div class="s1-img-1">
            <img src="@/assets/images/newpic/s3_card3_default.svg" alt="圖片" />
          </div>
          <div class="s1-img-2">
            <img src="@/assets/images/newpic/s3_card3_hover.svg" alt="圖片" />
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/mixin.scss";
@import "@/assets/scss/variables.scss";
@import "@/assets/scss/reset.scss";

.s1-title {
  width: 169.792px;
  height: 42.4px;
  margin: 0 auto;
  position: relative;

  @include min-width(768px) {
    width: 212.24px;
    height: 53.2px;
  }

  @include min-width(1440px) {
    width: 265.3px;
    height: 66.5px;
  }

  @include min-width(1920px) {
    width: 310px;
    height: 72px;
  }

  .h2 {
    width: 100%;
    height: 100%;
    display: block;
    position: absolute;
    top: 0px;
    left: 0px;
    background: url("@/assets/images/newpic/s2_START.svg") no-repeat
      center/contain;
    @include hidetext;
  }
}
.s1-content {
  margin-top: 6rem;
  position: relative;
  //border-top: 1px dashed $color-primary-1;
  //border-right: 1px dashed $color-primary-1;
  //border-top-right-radius: 50px;

  @include min-width(768px) {
    margin-top: 8rem;
  }

  @include min-width(1280px) {
    margin-top: 6rem;
  }

  @include min-width(1440px) {
    margin-top: 5rem;
  }
}
.s1-content-title-1 {
  width: 870px;
  margin: 0 auto;
  text-align: center;
  display: flex;
  flex-direction: column;

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

    &::after {
      content: "";
      display: block;
      position: absolute;
      top: -35px;
      left: 50%;
      margin-left: -131px;
      width: 262px;
      height: 48px;
      background: url("@/assets/images/newpic/s2_title.png") no-repeat;
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
      content: "";
      display: block;
      margin-top: -8px;
      position: absolute;
      top: 50%;
      left: 60px;
      width: 90px;
      height: 16px;
      background: url("@/assets/images/newpic/s0_line.svg") no-repeat;
      background-size: contain;
      background-position: 50% 50%;
    }

    &:before {
      content: "";
      display: block;
      margin-top: -8px;
      position: absolute;
      top: 50%;
      right: 60px;
      width: 90px;
      height: 16px;
      background: url("@/assets/images/newpic/s0_line.svg") no-repeat;
      background-size: contain;
      background-position: 50% 50%;
      transform: scaleX(-1);
    }
  }

  @include min-width(768px) {
  }

  @include min-width(1025px) {
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

  @include min-width(768px) {
  }

  @include min-width(1025px) {
  }

  &:before {
    content: "";
		position: absolute;
		top: -120px;
		left: -280px;
		width: 239px;
		height: 331px;
    display: block;
    background: url("@/assets/images/newpic/s3_bg_earphone.png") no-repeat;
    background-size: contain;
    background-position: 50% 50%;
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

    &::after {
      content: "";
      display: block;
      position: absolute;
      top: -35px;
      left: 50%;
      margin-left: -131px;
      width: 262px;
      height: 48px;
      background: url("@/assets/images/newpic/s3_title.png") no-repeat;
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
      content: "";
      display: block;
      margin-top: -8px;
      position: absolute;
      top: 50%;
      left: 60px;
      width: 90px;
      height: 16px;
      background: url("@/assets/images/newpic/s0_line.svg") no-repeat;
      background-size: contain;
      background-position: 50% 50%;
    }

    &:before {
      content: "";
      display: block;
      margin-top: -8px;
      position: absolute;
      top: 50%;
      right: 60px;
      width: 90px;
      height: 16px;
      background: url("@/assets/images/newpic/s0_line.svg") no-repeat;
      background-size: contain;
      background-position: 50% 50%;
      transform: scaleX(-1);
    }
  }
}
.s1-item-wrap {
  width: 80%;
  margin: 0 auto;
  margin-top: 6rem;

  @include min-width(1025px) {
    padding-bottom: 5rem;
    padding-left: 0;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  @include min-width(1280px) {
    margin-top: 6rem;
    padding-bottom: 3rem;
  }

  @include min-width(1440px) {
    padding-bottom: 5rem;
  }

  > li {
    width: 100%;
    margin-bottom: 3rem;

    &:last-child {
      margin-bottom: 0;
    }

    @include min-width(768px) {
      margin-bottom: 6rem;
    }

    @include min-width(1025px) {
      width: 30%;
      margin-bottom: 0;

      &:hover {
        .s1-img-1 {
          opacity: 0;
          display: none;
        }
        .s1-img-2 {
          opacity: 1;
          display: block;
        }
      }
    }

    @include min-width(1280px) {
      width: 28%;
    }

    .s1-img-1 {
      > img {
        width: 100%;
      }
    }

    .s1-img-2 {
      opacity: 0;
      display: none;

      > img {
        width: 100%;
      }
    }

    > .h3 {
      margin-top: 1.5rem;
      text-align: center;
      font-weight: 700;
      font-size: 22px;
      color: $color-primary-1;
    }

    .s1-info {
      margin-top: 2rem;
      line-height: 26px;
      font-weight: 400;
      font-size: 18px;
      text-align: center;
      color: $color-white;

      @include min-width(1025px) {
        font-size: 14px;
      }

      @include min-width(1280px) {
        font-size: 16px;
      }

      @include min-width(1440px) {
        font-size: 18px;
      }
    }
  }
}
.s1-item-2-wrap {
  position: relative;
  width: 80%;
  margin: 0 auto;
  margin-top: 6rem;

  @include min-width(1025px) {
    margin-top: 5rem;
    padding-left: 0;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  @include min-width(1280px) {
    margin-top: 6rem;
    padding-bottom: 3rem;
  }

  @include min-width(1440px) {
    padding-bottom: 5rem;
  }

  > li {
    width: 100%;
    margin-bottom: 2rem;
    position: relative;
    z-index: 5;

    @include min-width(768px) {
    }

    @include min-width(1025px) {
      width: 30%;
      margin-bottom: 0;

      &:hover {
        .s1-img-1 {
          opacity: 0;
          display: none;
        }
        .s1-img-2 {
          opacity: 1;
          display: block;
        }
      }
    }

    @include min-width(1280px) {
      width: 28%;
    }

    .s1-img-1 {
      > img {
        width: 100%;
      }
    }

    .s1-img-2 {
      opacity: 0;
      display: none;

      > img {
        width: 100%;
      }
    }
  }
}
</style>