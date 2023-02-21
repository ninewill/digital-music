<template>
  <div>
    <div class="s-title s1-title">
      <h2 class="h2">START</h2>
    </div>
    <div class="s-content s1-content">
      <div class="s1-content-title-1"></div>
      <ul class="s1-item-1">
        <li>
          <div class="s1-img-1">
            <img src="@/assets/images/pic/pic_01-1_photo.svg" alt="圖片" />
          </div>
          <div class="s1-img-2">
            <img src="@/assets/images/pic/pic_01-1_title.svg" alt="圖片" />
          </div>
          <p class="s1-info">
            零基礎至出片、有基礎至精進技法，用最短時間做出完美成品！
          </p>
        </li>
        <li>
          <div class="s1-img-1">
            <img src="@/assets/images/pic/pic_01-2_photo.svg" alt="圖片" />
          </div>
          <div class="s1-img-2">
            <img src="@/assets/images/pic/pic_01-2_title.svg" alt="圖片" />
          </div>
          <p class="s1-info">
            歌唱健檢、打穩基礎、提升技法，錄音室實戰，競賽彩排演出。
          </p>
        </li>
        <li>
          <div class="s1-img-1">
            <img src="@/assets/images/pic/pic_01-3_photo.svg" alt="圖片" />
          </div>
          <div class="s1-img-2">
            <img src="@/assets/images/pic/pic_01-3_title.svg" alt="圖片" />
          </div>
          <p class="s1-info">
            掌握比稿要領，知名講師引介管道，絕不讓自己吃虧，建立穩定收入。
          </p>
        </li>
      </ul>
      <div class="s1-content-title-2"></div>
      <ul class="s1-item-2">
        <li>
          <div class="s1-img-2">
            <img src="@/assets/images/pic/pic_02-1.svg" alt="圖片" />
          </div>
        </li>
        <li>
          <div class="s1-img-2">
            <img src="@/assets/images/pic/pic_02-2.svg" alt="圖片" />
          </div>
        </li>
        <li>
          <div class="s1-img-2">
            <img src="@/assets/images/pic/pic_02-3.svg" alt="圖片" />
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
    width: 379px;
    height: 95px;
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
  border-top: 1px dashed $color-primary-1;
  border-right: 1px dashed $color-primary-1;
  border-top-right-radius: 50px;

	@include min-width(768px) {
		margin-top: 8rem;
	}

  @include min-width(1280px) {
    margin-top: 6rem;
  }

  @include min-width(1440px) {
    margin-top: 8rem;
  }
}
.s1-content-title-1 {
  position: absolute;
  top: 0;
  margin-top: -19%;
  width: 88%;
  padding-bottom: 30.769%;
  background: url("@/assets/images/pic/mobile/pic_01_title01.svg") no-repeat;
  background-size: contain;
  background-position: 0 100%;

  @include min-width(768px) {
    width: 50%;
    margin-top: -23%;
  }

  @include min-width(1025px) {
    width: 100%;
    margin-top: -7%;
    padding-bottom: 12.85%;
    background: url("@/assets/images/pic/pic_01_title.svg") no-repeat;
    background-size: contain;
  }
}
.s1-content-title-2 {
  width: 88%;
  margin: 0 auto;
  padding-bottom: 34.32%;
  background: url("@/assets/images/pic/mobile/pic_02_title02.svg") no-repeat;
  background-size: contain;
  background-position: 50% 50%;

  @include min-width(768px) {
    width: 50%;
  }

  @include min-width(1025px) {
    width: 100%;
    margin-top: 0%;
    padding-bottom: 12.85%;
    background: url("@/assets/images/pic/pic_02_title.svg") no-repeat;
    background-size: contain;
    background-position: 0 100%;
  }
}
.s1-item-1 {
  margin-top: 6rem;
  padding-right: 1.5rem;
  padding-left: 1.5rem;

  @include min-width(1025px) {
    padding-bottom: 5rem;
    padding-right: 2rem;
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
    margin-top: 9rem;
    padding-bottom: 5rem;
    padding-right: 5rem;
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
      width: 32%;
      margin-bottom: 0;
    }

    @include min-width(1280px) {
      width: 31.5%;
    }

    .s1-img-1 {
      > img {
        width: 100%;
      }
    }

    .s1-img-2 {
      margin-top: 1rem;

      @include min-width(768px) {
        margin-top: 3rem;
      }

      @include min-width(1025px) {
        margin-top: 1rem;
      }

      > img {
        width: 100%;
      }
    }

    .s1-info {
      margin-top: 1rem;
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
.s1-item-2 {
  position: relative;
  padding-right: 3rem;
  padding-left: 3rem;
  padding-bottom: 3.8rem;

  @include min-width(1025px) {
    margin-top: 5rem;
    padding-right: 2rem;
    padding-left: 0;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  @include min-width(1280px) {
    margin-top: 3rem;
  }

  @include min-width(1440px) {
    margin-top: 5rem;
  }

  &:after {
    content: "";
    display: block;
    width: 188.3px;
    height: 206.5px;
    position: absolute;
    bottom: -49px;
    right: 0;
    background: url("@/assets/images/pic/pic_02-4_people.svg") no-repeat;
    background-size: contain;
    background-position: 50% 50%;
		z-index: 10;

    @include min-width(1025px) {
      width: 188.3px;
      height: 206.5px;
      right: 8%;
      top: -45%;
      bottom: auto;
    }

    @include min-width(1440px) {
      width: 210px;
      height: 295px;
      right: 8%;
      top: -47%;
    }

    @include min-width(1920px) {
      width: 269px;
      height: 308px;
      right: 5%;
    }
  }

  > li {
    width: 100%;
    margin-bottom: 2rem;
    position: relative;
    z-index: 5;

    @include min-width(1025px) {
      width: 30%;
      margin-bottom: 0;

      &::after {
        content: "";
        width: 50px;
        height: 50px;
        position: absolute;
        top: 50%;
        right: -19%;
        display: block;
        background: url("@/assets/images/pic/pic_02-5_cross.svg") no-repeat;
        background-size: contain;
        background-position: 0 100%;

        @include min-width(1025px) {
          width: 40px;
          height: 40px;
          right: -20%;
        }

        @include min-width(1440px) {
          width: 50px;
          height: 50px;
          right: -19%;
        }
      }

      &:last-child {
        &::after {
          display: none;
        }
      }
    }

    .s1-img-2 {
      > img {
        width: 100%;
      }
    }
  }
}
</style>