<template>
  <div>
    <div class="s3-content-title-2">
      <div class="h3">全方位解鎖數位成音技能，升職加薪進度條滿格加載</div>
      <span class="s1-description"
        >音效配樂規模強與吸金力躍進，音樂人才需求量大</span
      >
    </div>
    <div class="salary-chart">
      <div class="salary-title">
        <div class="salary-title-img">
          <img src="@/assets/images/newpic/s6_SALARY.svg" alt="圖片" />
        </div>
      </div>
      <div class="salary-wrap">
        <div class="salary-info">
          <div class="h4">數位成音業界基本薪資分布</div>
          <p>
            隨著數位化的浪潮，數位成音是現代具影響力的新趨勢，音樂產業或成千上萬大產業，音效、配樂、配音、混音、微電影皆無處不在，人們獲取信息的渠道與方式從未停止變化，掌握數位成音技能，既可獨自承接專案項目也可邁向就業道路，實現更多在工作上的自主權！
          </p>
        </div>
        <div class="salary-chart-bar">
          <Chart />
          <ul class="salary-num">
            <li>$42,000~</li>
            <li>$35,000~</li>
            <li>$35,000~</li>
            <li>$35,000~</li>
            <li>$30,000~</li>
            <li>$10,000~</li>
            <li>$5,000~</li>
            <li>$3,000~</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Chart from '@/components/Chart.vue';

export default {
  components: {
    Chart,
  },
};
</script>

<style lang="scss" scoped>
@import '@/assets/scss/mixin.scss';
@import '@/assets/scss/variables.scss';
@import '@/assets/scss/reset.scss';
@import '@/assets/scss/animate.scss';

.s3-content-title-2 {
  width: 870px;
  margin: 0 auto;
  position: relative;
  margin-top: 5rem;
  text-align: center;
  display: flex;
  flex-direction: column;

  &:before {
    @include min-width(1280px) {
      content: '';
      position: absolute;
      top: -120px;
      left: -280px;
      width: 192px;
      height: 192px;
      display: block;
      background: url('@/assets/images/newpic/s6_bg_deco.png') no-repeat;
      background-size: contain;
      background-position: 50% 50%;
    }
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

    &::before {
      content: '';
      display: block;
      position: absolute;
      top: -35px;
      left: 50%;
      margin-left: -131px;
      width: 262px;
      height: 48px;
      background: url('@/assets/images/newpic/s6_title.png') no-repeat;
      background-size: contain;
      background-position: 50% 50%;
    }

    &::after {
      @include min-width(1280px) {
        content: '';
        display: block;
        position: absolute;
        top: 50px;
        right: -20%;
        width: 124px;
        height: 140px;
        background: url('@/assets/images/newpic/s6_note.png') no-repeat;
        background-size: contain;
        background-position: 50% 50%;
        animation: musicBounce 2.8s ease-in-out infinite;
      }
    }
  }
  > .s1-description {
    margin-top: 1.5rem;
    position: relative;
    display: block;
    font-size: 24px;
    color: $color-white;

    &::after {
      content: '';
      display: block;
      margin-top: -8px;
      position: absolute;
      top: 50%;
      left: 60px;
      width: 90px;
      height: 16px;
      background: url('@/assets/images/newpic/s0_line.svg') no-repeat;
      background-size: contain;
      background-position: 50% 50%;
    }

    &:before {
      content: '';
      display: block;
      margin-top: -8px;
      position: absolute;
      top: 50%;
      right: 60px;
      width: 90px;
      height: 16px;
      background: url('@/assets/images/newpic/s0_line.svg') no-repeat;
      background-size: contain;
      background-position: 50% 50%;
      transform: scaleX(-1);
    }
  }
}

.salary-chart {
  &::after {
    content: '';
    display: block;
    position: absolute;
    right: 0;
    bottom: -100px;
    width: 95%;
    border: 1px dashed $color-primary-1;
  }
  .salary-title {
    position: relative;
    margin-top: 5rem;
    padding: 0 5rem;
    display: flex;
    align-items: center;

    .salary-title-img {
      width: 40%;

      @include min-width(1025px) {
        width: 40%;
      }

      @include min-width(1440px) {
        width: 40%;
      }

      > img {
        width: 100%;
      }
    }

    @include min-width(1025px) {
      padding: 0 2rem;
    }

    @include min-width(1440px) {
      padding: 0 5rem;
    }

    &::after {
      content: '';
      display: block;
      position: absolute;
      right: 0;
      width: 60%;
      border: 1px dashed $color-primary-1;

      @include min-width(1025px) {
        width: 50%;
      }

      @include min-width(1440px) {
        width: 55%;
      }
    }
  }
}

.salary-wrap {
  margin-top: 5rem;
  padding: 0 5rem;
  display: flex;
  justify-content: space-between;

  @include min-width(1280px) {
    padding: 0 2rem;
    padding-right: 0;
  }

  @include min-width(1440px) {
    padding: 0 5rem;
  }

  .salary-info {
    width: 35%;
    padding: 2.5rem;
    border: 1px solid $color-primary-1;
    border-radius: 20px;
    position: relative;

    @include min-width(1280px) {
      padding: 2.5rem 1.5rem;
    }

    @include min-width(1440px) {
      padding: 2.5rem;
    }

    &::after {
      content: '';
      width: 73px;
      height: 73px;
      position: absolute;
      top: -35px;
      left: -35px;
      display: block;
      background: url('@/assets/images/newpic/s6_star.png') no-repeat
        center/contain;
    }

    > .h4 {
      color: $color-primary-1;
      font-size: 1.2vw;

      @include min-width(1280px) {
        font-size: 1.6vw;
      }

      @include min-width(1440px) {
        font-size: 1.5vw;
      }

      @include min-width(1650px) {
        font-size: 1.3vw;
      }

      @include min-width(1920px) {
        font-size: 1vw;
      }
    }

    > p {
      margin-top: 1rem;
      margin-bottom: 0;
      line-height: 2em;
      color: $color-white;
      font-size: 0.9vw;

      @include min-width(1280px) {
        font-size: 1.1vw;
      }

      @include min-width(1440px) {
        font-size: 1vw;
      }

      @include min-width(1650px) {
        font-size: 0.9vw;
      }

      @include min-width(1920px) {
        font-size: 0.8vw;
      }
    }
  }

  .salary-chart-bar {
    width: 60%;
    position: relative;

    .salary-num {
      margin-top: 1rem;
      position: absolute;
      top: 0;
      right: -50px;

      @include min-width(1280px) {
        display: none;
      }

      @include min-width(1440px) {
        display: block;
        right: -70px;
      }

      @include min-width(1650px) {
        right: -80px;
      }

      @include min-width(1920px) {
        right: -150px;
      }

      > li {
        margin-top: 1.3rem;
        color: $color-primary-1;
        font-size: 0.9vw;

        &:first-child {
          margin-top: 0;
        }

        @include min-width(1025px) {
          font-size: 1.2vw;
        }

        @include min-width(1440px) {
          margin-top: 1rem;
          font-size: 1.1rem;
        }

        @include min-width(1920px) {
          margin-top: 1.3rem;
          font-size: 0.9vw;
        }
      }
    }
  }
}
</style>
