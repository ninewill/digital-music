<template>
  <div>
    <div class="s1-content-title-2">
      <div class="h3">學配音、音效、混音、錄音，首選赫綵</div>
      <span class="s1-description"
        >全方位數位成音課程，讓你與業界無縫接軌！</span
      >
    </div>
    <ul class="best-item">
      <li>
        <div class="s5-img-1">
          <img src="@/assets/images/newpic/s7_p1.png" alt="圖片" />
        </div>
        <div class="h3">電視台參訪</div>
        <p>實際參訪相關領域，熟悉業界 運作流程。</p>
      </li>
      <li>
        <div class="s5-img-2">
          <img src="@/assets/images/newpic/s7_p1.png" alt="圖片" />
        </div>
        <div class="h3">動畫配音工作室</div>
        <p>體驗動畫配音，專業業師傳授 實戰經驗。</p>
      </li>
      <li>
        <div class="s5-img-3">
          <img src="@/assets/images/newpic/s7_p1.png" alt="圖片" />
        </div>
        <div class="h3">知名業師引薦</div>
        <p>業界知名配音員、混音師、錄音師，引薦公司接案管道。</p>
      </li>
      <li>
        <div class="s5-img-4">
          <img src="@/assets/images/newpic/s7_p1.png" alt="圖片" />
        </div>
        <div class="h3">教學品質保證</div>
        <p>全方位專業課程教學，最高規格 電腦設備教室。</p>
      </li>
    </ul>
  </div>
</template>

<script>
//import Chart from "@/components/Chart.vue";

export default {
  components: {
    //Chart,
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
    left: -500px;
    width: 316px;
    height: 360px;
    display: block;
    background: url("@/assets/images/newpic/s7_bg_deco.png") no-repeat;
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

.best-item {
  margin-top: 5rem;
  display: flex;
  justify-content: space-between;

  > li {
    width: 24%;

    img {
      width: 100%;
    }
  }
}
</style>