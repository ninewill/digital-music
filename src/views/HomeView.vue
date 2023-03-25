<template>
  <!--main-->
  <div id="main" class="wrap wrap-content">
    <section class="section-block section0">
      <IndexBlock />
    </section>
    <!--START-->
    <section id="1" class="section-block section1">
      <StartBlock />
    </section>
    <!--COURSE-->
    <section class="section-block section2">
      <CourseBlock />
    </section>
    <!--COURSE Card slide-->
    <div id="2" class="section-block section2-1">
      <CourseBlock2 />
    </div>
    <!--Training Center-->
    <section class="section-block section3">
      <TrainingCenter />
    </section>
    <div class="tc-bar">
      <TrainingCenterBar />
    </div>
    <!--SALARY-->
    <section class="section-block section4">
      <Salary />
    </section>
    <!--BEST CHOICE-->
    <section class="section-block section5">
      <BestChoice />
    </section>
    <!--BONUS Bar-->
    <div class="bonus-bar"></div>
    <!--BonusBlock-->
    <section class="section-block section6">
      <BonusBlock />
    </section>
    <!-- BEST COURSE WAVE -->
    <div class="wave"></div>
    <!--BEST COURSE-->
    <div id="3" class="section-block course-block">
      <BestCourse />
    </div>
    <!--Reply-->
    <section class="section7">
      <Reply />
    </section>
  </div>
  <Cursor />
</template>

<script>
import IndexBlock from '@/components/IndexBlock.vue';
import StartBlock from '@/components/StartBlock.vue';
import CourseBlock from '@/components/CourseBlock.vue';
import CourseBlock2 from '@/components/CourseBlock2.vue';
import TrainingCenter from '@/components/TrainingCenter.vue';
import TrainingCenterBar from '@/components/TrainingCenterBar.vue';
import Salary from '@/components/Salary.vue';
import BestChoice from '@/components/BestChoice.vue';
import BonusBlock from '@/components/BonusBlock.vue';
import BestCourse from '@/components/BestCourse.vue';
import Reply from '@/components/Reply.vue';
import Swiper from '@/components/Swiper.vue';
import Cursor from '@/components/Cursor.vue';

export default {
  components: {
    IndexBlock,
    StartBlock,
    CourseBlock,
    CourseBlock2,
    TrainingCenter,
    TrainingCenterBar,
    Salary,
    BestChoice,
    BonusBlock,
    BestCourse,
    Reply,
    Swiper,
    Cursor,
  },
  mounted() {},
};
</script>

<style lang="scss">
@import '@/assets/scss/mixin.scss';
@import '@/assets/scss/variables.scss';
@import '@/assets/scss/reset.scss';

.section-block {
  width: calc(100% - 40px);
  margin: 0 auto;

  @include min-width(525px) {
    width: calc(100% - 60px);
  }

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

  > h1 {
    font-size: 80px;
    color: $color-white;
  }
}

.s-content {
  position: relative;
}

.section0 {
  position: relative;

  &::after {
    content: '';
    width: 20px;
    height: 436px;
    display: block;
    position: absolute;
    top: 120px;
    right: 0px;
    background: url('@/assets/images/newpic/s0_deco_text.svg') no-repeat
      center/cover;
  }
}

.section1 {
  position: relative;
  margin-top: 5rem;

  @include min-width(1025px) {
    margin-top: 5rem;

    &::before {
      content: '';
      width: 147px;
      height: 153px;
      display: block;
      position: absolute;
      top: -50px;
      left: 0;
      background: url('@/assets/images/newpic/s2_bg_deco01.svg') no-repeat
        center/contain;
    }

    &::after {
      content: '';
      width: 200px;
      height: 200px;
      display: block;
      position: absolute;
      top: 0px;
      right: 0;
      background: url('@/assets/images/newpic/s2_bg_deco02.svg') no-repeat
        center/contain;
    }
  }

  @include min-width(1280px) {
    &::before {
      top: -100px;
      left: -50px;
    }

    &::after {
      top: 0px;
      right: -100px;
    }
  }

  @include min-width(1440px) {
    &::before {
      top: -50px;
    }

    &::after {
      top: 0px;
    }
  }
}
.section2 {
  margin-top: 5rem;
  position: relative;
}

.section2-1 {
  margin-top: 5rem;
  position: relative;

  @include min-width(768px) {
    margin-top: 15rem;
  }

  &::after {
    @include min-width(1280px) {
      content: '';
      display: block;
      width: 200px;
      height: 600px;
      position: absolute;
      top: -200px;
      right: -25%;
      background: url('@/assets/images/newpic/s4_bg_micro.png') no-repeat
        center/contain;
    }
  }
}
.s2-content-silde {
  margin-top: 3rem;
  position: relative;
  border-bottom: 2px solid $color-primary-1;

  @include min-width(1025px) {
    margin-top: 15rem;
  }

  &:after {
    content: '';
    display: block;
    position: absolute;
    left: 50%;
    width: 0;
    height: 0;
    margin-left: -15px;
    border-style: solid;
    border-width: 26px 15px 0 15px;
    border-color: $color-primary-1 transparent transparent transparent;

    @include min-width(768px) {
      border-width: 35px 24px 0 24px;
      margin-left: -24px;
    }
  }

  .s2-content-silde-title {
    width: 90%;
    margin: 0 auto;

    @include min-width(768px) {
      width: 70%;
    }

    @include min-width(1025px) {
      width: 50%;
    }

    > img {
      width: 100%;
    }
  }
}

.section3 {
  margin-top: 5rem;
  position: relative;

  @include min-width(768px) {
    margin-top: 15rem;
  }

  @include min-width(1025px) {
    margin-top: 18rem;
  }
}
.section4 {
  margin-top: 6rem;
  position: relative;

  @include min-width(1025px) {
    margin-top: 12rem;
  }
}

.section5 {
  margin-top: 15rem;
  position: relative;
}

.section6 {
  margin-top: 0rem;
  position: relative;

  @include min-width(1025px) {
    margin-top: 15rem;
  }
}

.section7 {
  position: relative;

  @include min-width(1025px) {
    margin-top: 50rem;
  }

  @include min-width(1440px) {
    margin-top: 55rem;
  }

  @include min-width(1650px) {
    margin-top: 50rem;
  }

  @include min-width(1920px) {
    margin-top: 35rem;
  }
}

.tc-bar {
  padding: 40px;
  border-top: 1px solid $color-primary-1;
  border-bottom: 1px solid $color-primary-1;

  @include min-width(484px) {
    padding: 3.75rem 10rem 3.75rem 5rem;
  }

  @include min-width(768px) {
    padding: 3.75rem 16rem;
  }

  @include min-width(960px) {
    padding: 3.75rem 18rem;
  }

  @include min-width(1025px) {
    padding: 3.75rem 0;
  }
}

.bonus-bar {
  margin-top: 5rem;
  border-top: 1px solid $color-primary-1;
  position: relative;
  display: flex;
  justify-content: center;

  &::after {
    content: '';
    position: absolute;
    display: block;
    width: 170px;
    height: 57px;
    background: url('@/assets/images/newpic/s7_arrow.svg') no-repeat
      center/contain;
  }
}

.course-block {
  position: relative;
  // height: 800px;
}

.wave {
  @include min-width(1025px) {
    margin-top: 20rem;
    width: 100%;
    padding-bottom: 42.9%;
    background: url('@/assets/images/newpic/s9_bg_line.png') no-repeat
      center/cover;
  }

  @include min-width(1280px) {
    margin-top: 15rem;
  }

  @include min-width(1440px) {
    margin-top: 20rem;
  }

  @include min-width(1650px) {
    margin-top: 17rem;
  }

  @include min-width(1920px) {
    margin-top: 15rem;
  }
}
</style>
