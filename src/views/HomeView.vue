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
    <!--Border Line-->
    <div class="section-block border-line">
      <span></span>
      <span class="radius radius-r"></span>
      <span class="radius radius-l"></span>
      <span></span>
    </div>
    <!--COURSE-->
    <section class="section-block section2">
      <CourseBlock />
    </section>
    <!--COURSE Card slide-->
    <div id="2" class="s2-content-silde">
      <div class="s2-content-silde-title">
        <img src="@/assets/images/pic/pic_05_title.svg" alt="圖片" />
      </div>
      <Swiper />
    </div>
    <!--STUDENT WORKS-->
    <section class="section-block section3">
      <StudentWorksBlock />
    </section>
    <!--DREAM ON-->
    <section class="section-block section4">
      <DreamOnBlock />
    </section>
    <div class="music-bar">
      MUSIC IS A KIND OF POWER · MUSIC IS A KIND OF POWER
    </div>
    <div id="3" class="section4-wrapp">
      <div class="section-block">
        <DreamOnBlock_1 />
      </div>
      <div class="section-block-1">
        <DreamOnBlock_2 />
      </div>
    </div>
    <!--WITNESS-->
    <section class="witness-block section5">
      <Witness />
    </section>
  </div>
</template>

<script>
import IndexBlock from "@/components/IndexBlock.vue";
import StartBlock from "@/components/StartBlock.vue";
import CourseBlock from "@/components/CourseBlock.vue";
import StudentWorksBlock from "@/components/StudentWorksBlock.vue";
import DreamOnBlock from "@/components/DreamOnBlock.vue";
import DreamOnBlock_1 from "@/components/DreamOnBlock-1.vue";
import DreamOnBlock_2 from "@/components/DreamOnBlock-2.vue";
import Witness from "@/components/Witness.vue";
import Swiper from "@/components/Swiper.vue";

export default {
  components: {
    IndexBlock,
    StartBlock,
    CourseBlock,
    StudentWorksBlock,
    DreamOnBlock,
    DreamOnBlock_1,
    DreamOnBlock_2,
    Witness,
    Swiper,
  },
};
</script>

<style lang="scss">
@import "@/assets/scss/mixin.scss";
@import "@/assets/scss/variables.scss";
@import "@/assets/scss/reset.scss";

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

//Border Line
.border-line {
  display: flex;
  flex-wrap: wrap;

  > span {
    display: block;
    width: 50%;
    height: 50px;

    &.radius {
      border-color: $color-primary-1;
      border-width: 1px;
    }

    &.radius-r {
      border-bottom-style: dotted;
      border-right-style: dotted;
      border-bottom-right-radius: 50px;
    }

    &.radius-l {
      border-top-style: dotted;
      border-left-style: dotted;
      border-top-left-radius: 50px;
    }
  }
}

.section0{
	position: relative;


	&::after{
		content: "";
		width: 20px;
		height: 436px;
		display: block;
		position: absolute;
		top: 80px;
		right:0px;
		background: url("@/assets/images/newpic/s0_deco_text.svg") no-repeat
      center/cover;
	}
}

.section1 {
	position: relative;

	@include min-width(1025px) {
    &::before{
			content: "";
			width: 147px;
			height: 153px;
			display: block;
			position: absolute;
			top: -50px;
			left: 0;
			background: url("@/assets/images/newpic/s2_bg_deco01.svg") no-repeat
      center/contain;
		}

		&::after{
			content: "";
			width: 200px;
			height: 200px;
			display: block;
			position: absolute;
			top: 0px;
			right: 0;
			background: url("@/assets/images/newpic/s2_bg_deco02.svg") no-repeat
      center/contain;
		}
  }

  @include min-width(1280px) {
    margin-top: 3rem;
  }

  @include min-width(1440px) {
    margin-top: 5rem;
  }
}
.section2 {
  position: relative;
}
.s2-content-silde {
  margin-top: 3rem;
  position: relative;
  border-bottom: 2px solid $color-primary-1;

  @include min-width(1025px) {
    margin-top: 6rem;
  }

  &:after {
    content: "";
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
  margin-top: 12rem;
  position: relative;

  @include min-width(768px) {
    margin-top: 20rem;
  }

  @include min-width(1025px) {
    margin-top: 23rem;
  }
}
.section4 {
  margin-top: 12rem;
  position: relative;
}

.music-bar {
  margin-top: 3rem;
  padding: 1rem 0;
  font-weight: 800;
  font-size: 18px;
  color: $color-white;
  text-align: center;
  background: linear-gradient(137.1deg, #fff176 14.56%, #00e0b8 85.34%);

  @include min-width(1025px) {
    margin-top: 7rem;
    padding: 2rem 0;
    font-size: 30px;
  }

  @include min-width(1440px) {
    font-size: 40px;
  }

  @include min-width(1920px) {
    font-size: 50px;
  }
}

.witness-block {
  padding-bottom: 3rem;
  position: relative;
  border-image: linear-gradient(to right, #fff176, #00e0b8) 30;
  border-top: 1px solid;
  border-bottom: 1px solid;

  @include min-width(1025px) {
    padding-bottom: 0;
  }
}
</style>