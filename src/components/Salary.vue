<template>
  <div>
    <div class="s1-content-title-2">
      <div class="h3">全方位解鎖數位成音技能，升職加薪進度條滿格加載</div>
      <span class="s1-description"
        >音效配樂規模強與吸金力躍進，音樂人才需求量大</span
      >
    </div>
    <div class="salary-chart">
      <div class="salary-title">
        <img src="@/assets/images/newpic/s6_SALARY.svg" alt="圖片" />
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
import Chart from "@/components/Chart.vue";

export default {
  components: {
    Chart,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/mixin.scss";
@import "@/assets/scss/variables.scss";
@import "@/assets/scss/reset.scss";
@import "@/assets/scss/animate.scss";

.s1-content-title-2 {
  width: 870px;
  margin: 0 auto;
  position: relative;
  margin-top: 5rem;
  text-align: center;
  display: flex;
  flex-direction: column;

  &:before {
    content: "";
    position: absolute;
    top: -120px;
    left: -280px;
    width: 192px;
    height: 192px;
    display: block;
    background: url("@/assets/images/newpic/s6_bg_deco.png") no-repeat;
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

    &::before {
      content: "";
      display: block;
      position: absolute;
      top: -35px;
      left: 50%;
      margin-left: -131px;
      width: 262px;
      height: 48px;
      background: url("@/assets/images/newpic/s6_title.png") no-repeat;
      background-size: contain;
      background-position: 50% 50%;
    }

    &::after {
      content: "";
      display: block;
      position: absolute;
      top: 50px;
      right: -20%;
      width: 124px;
      height: 140px;
      background: url("@/assets/images/newpic/s6_note.png") no-repeat;
      background-size: contain;
      background-position: 50% 50%;
      animation: musicBounce 2.8s ease-in-out infinite;
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

.salary-chart {

	&::after {
      content: "";
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

    &::after {
      content: "";
      display: block;
      position: absolute;
      right: 0;
      width: 60%;
      border: 1px dashed $color-primary-1;
    }
  }
}

.salary-wrap {
  margin-top: 5rem;
  padding: 0 5rem;
  display: flex;
  justify-content: space-between;

  .salary-info {
    width: 35%;
    padding: 2.5rem;
    border: 1px solid $color-primary-1;
    border-radius: 20px;

    > .h4 {
      color: $color-primary-1;
      font-size: 1.2vw;
    }

    > p {
      margin-top: 1rem;
      margin-bottom: 0;
      line-height: 2em;
      color: $color-white;
      font-size: 0.9vw;
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
					font-size: 0.9vw;
        }

        @include min-width(1920px) {
          margin-top: 1.3rem;
        }
      }
    }
  }
}
</style>