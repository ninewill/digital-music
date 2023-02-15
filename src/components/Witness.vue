<template>
  <div class="section5-block">
    <div class="section5-block-title">
      <h2 class="h2">WITNESS</h2>
    </div>
    <ul class="section5-item">
      <li>
        <div class="s5-container">
          <div class="s5-title">
            <h3 class="h3">音樂製作人課程</h3>
            <span>台中學院｜學員 張Ｏ芝</span>
          </div>
          <div class="s5-text-wrap">
            <p>
              阿樂老師和Mike上課都非常非常豐富、認真和有耐心，每堂課都能有許多不一樣的收穫，讓身為學生的我感到很幸福。
            </p>
            <p>
              自己是非本科的背景，即使有涉略過樂器和音樂歌唱，但一剛開始真的仍然會覺得很有難度（軟體操作），這確實需要反覆多次練習理解才能進入狀況。不過整體來說收穫至少也有60%~70%，最起碼知道老師在表達的邏輯、緣由、和目標方向是什麼，其實很好玩，也很喜歡，覺得慶幸自己沒有還是走到了最後，相信能不斷複習和重修的話，應該會更有機會進步，謝謝各位老師和助教。
            </p>
          </div>
          <div class="s5-bottom">
            <div class="star">
              <img src="@/assets/images/pic/pic_09-1_star.svg" alt="圖片" />
            </div>
            <div class="date">2021.12.</div>
          </div>
        </div>
      </li>
      <li>
        <div class="s5-container">
          <div class="s5-title">
            <h3 class="h3">音樂製作人課程</h3>
            <span>台中學院｜學員 林Ｏ潔</span>
          </div>
          <div class="s5-text-wrap">
            <p>
              Mia和暄超棒的，好喜歡她們。老師很都很專業，很棒，謝謝三位老師在課後回答問題，有時候課堂上會不好意思問。
            </p>
            <p>
              謝謝阿樂老師、謝謝佑龍老師在課堂上詢問大家關於音樂職涯發展的想法，也幫我釐清一些方向。謝謝Mike老師，想再多聽一些怎麼幫動畫、影片或有聲書配樂。
            </p>
            <p>
              課程：老師分享很多業界的眉角，覺得可以聽到很多很棒，像評審方式和製作經驗，感覺自己平常很難接觸的到。不過如果編曲部分時間可以再長一些就更棒了。
            </p>
          </div>
          <div class="s5-bottom">
            <div class="star">
              <img src="@/assets/images/pic/pic_09-1_star.svg" alt="圖片" />
            </div>
            <div class="date">2021.12.</div>
          </div>
        </div>
      </li>
      <li>
        <div class="s5-container">
          <div class="s5-title">
            <h3 class="h3">音樂製作人課程</h3>
            <span>台中學院｜學員 張Ｏ翔</span>
          </div>
          <div class="s5-text-wrap">
            <p>
              首先感謝赫綵提供這麼棒的課程跟師資，讓我真的有在音樂專業的班級訓練的感覺，專業知識及操作，教學上都非常到位，師資群都非常用心，不論是課程指導方面、協助同學解惑方面、甚至到後續關心同學操作軟體或寫歌等等狀況，還有助教也會隨時協助同學排除困難。
            </p>
            <p>
              音樂製作人的課程，讓我過了非常充實的72小時，也成功寫出了一首自己很喜歡的作品，謝謝赫綵設計規畫這個課程，謝謝授課老師們，還有謝謝我的兩位超優質顧問，我會好好期待接下來的詞曲創作以及錄音室歌唱這些課程的。謝謝你們。
            </p>
          </div>
          <div class="s5-bottom">
            <div class="star">
              <img src="@/assets/images/pic/pic_09-1_star.svg" alt="圖片" />
            </div>
            <div class="date">2021.12.</div>
          </div>
        </div>
      </li>
      <li>
        <div class="s5-container">
          <div class="s5-title">
            <h3 class="h3">音樂製作人課程</h3>
            <span>台中學院｜學員 陳Ｏ仁</span>
          </div>
          <div class="s5-text-wrap">
            <p>
              第一次進到赫綵上課，感覺很開心，能認識這些同學和那麼專業的老師是我的榮幸，能和同學們一起完成一首歌的感覺真的很棒，但因為工作的關係，常常都上完大夜班後接著上課，會因為精神和體力消耗太多而恍神，但還好有carry的同學們幫忙，真的很謝謝他們，也謝謝老師們細心的指導。
            </p>
          </div>
          <div class="s5-bottom">
            <div class="star">
              <img src="@/assets/images/pic/pic_09-1_star.svg" alt="圖片" />
            </div>
            <div class="date">2021.12.</div>
          </div>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/mixin.scss";
@import "@/assets/scss/variables.scss";
@import "@/assets/scss/reset.scss";

.section5-block {
  width: calc(100% - 40px);
  margin: 0 auto;
  position: relative;

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
}

.section5-block-title {
  width: 202px;
  height: 37px;
  position: absolute;
  top: 0;
  left: 50%;
  margin-top: -28%;
  margin-left: -101px;
  z-index: 1;

  @include min-width(1025px) {
    width: 193.6px;
    height: 32.8px;
    left: 0;
    margin-top: -10%;
    margin-left: 0;
  }

  @include min-width(1440px) {
    width: 242.2px;
    height: 41.3px;
    margin-top: -8%;
  }

  @include min-width(1920px) {
    width: 346px;
    height: 59px;
  }

  .h2 {
    width: 100%;
    height: 100%;
    display: block;
    position: absolute;
    top: 0px;
    left: 0px;
    background: url("@/assets/images/pic/pic_09_WITNESS.svg") no-repeat
      center/contain;
    @include hidetext;
  }
}

.section5-item {
  margin-top: 5rem;
  display: flex;
  justify-content: space-between;

  @include max-width(1025px) {
    overflow-x: auto;
    flex-wrap: nowrap;
  }

  > li {
    margin-right: 1rem;
    flex: none;
    width: 100%;
    position: relative;
    border-radius: 20px;
    background-image: linear-gradient(to right, #fff176, #00e0b8);

    @include min-width(1025px) {
      width: 24%;
      margin-right: 0;
      top: 2rem;
    }

    .s5-container {
      //min-height: 483px;
      display: flex;
      flex-direction: column;
      margin: 2px;
      padding: 2rem 1.5rem;
      border-radius: 19px;
      background-color: $color-black;

      .s5-title {
        margin-bottom: 1.5rem;
        padding-bottom: 1rem;
        border-image: linear-gradient(to right, #fff176, #00e0b8) 30;
        border-bottom: 1px solid;

        .h3 {
          font-weight: 700;
          font-size: 26px;
          background: linear-gradient(137.1deg, #fff176 14.56%, #00e0b8 85.34%);
          background-clip: text;
          color: transparent;

          @include min-width(1025px) {
            font-size: 20px;
          }

          @include min-width(1440px) {
            font-size: 22px;
          }

          @include min-width(1920px) {
            font-size: 26px;
          }
        }

        > span {
          margin-top: 1rem;
          display: block;
          color: $color-white;
        }
      }

      .s5-text-wrap {
				height: 350px;
        margin-bottom: 2rem;

        @include min-width(1025px) {
          height: 150px;
          overflow-y: auto;
        }

        @include min-width(1440px) {
          height: 200px;
        }

        @include min-width(1920px) {
          height: 275px;
        }

        > p {
          font-weight: 400;
          font-size: 16px;
          color: $color-white;

          &:last-child {
            margin-bottom: 0;
          }

					@include min-width(1025px) {
						font-size: 12px;
					}

          @include min-width(1920px) {
            font-size: 13px;
          }
        }
      }

      .s5-bottom {
        margin-top: auto;
        display: flex;
        justify-content: space-between;

        .date {
          color: $color-white;
        }
      }
    }
  }
}
</style>