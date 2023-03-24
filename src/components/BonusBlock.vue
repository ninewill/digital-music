<template>
  <div>
    <div class="s-content s4-content">
      <FormSingle />
    </div>
    <a href="#4" class="btn-course">
      <img
        class="btn-def"
        src="@/assets/images/newbtn/s0_coures_default.png"
        alt="圖片"
      />
      <img
        class="btn-hover"
        src="@/assets/images/newbtn/s0_coures_hover.png"
        alt="圖片"
      />
    </a>
  </div>
</template>

<script>
import FormSingle from '@/components/FormSingle.vue';

export default {
  components: {
    FormSingle,
  },
  mounted() {
    $('.btn-course').click(function () {
      let target = this.hash,
        $target = $(target).offset().top;

      $('html, body').animate({ scrollTop: $target }), 1500;
    });
  },
};
</script>

<style lang="scss" scoped>
@import '@/assets/scss/mixin.scss';
@import '@/assets/scss/variables.scss';
@import '@/assets/scss/reset.scss';

.s4-title {
  width: 240px;
  height: 35.2px;
  left: 50%;
  margin-left: -120px;
  position: absolute;
  top: -6%;
  z-index: 1;

  @include min-width(768px) {
    width: 301px;
    height: 44px;
    left: 50%;
    top: -8%;
    margin-left: -150.5px;
  }

  @include min-width(1025px) {
    top: -8%;
    left: 0;
    margin-left: 0;
  }

  @include min-width(1440px) {
    width: 377.3px;
    height: 55.3px;
    margin-left: 100px;
    top: -12%;
  }

  @include min-width(1920px) {
    width: 539px;
    height: 79px;
    top: -15%;
  }
}

.btn-course {
  width: 84.7px;
  height: 97.3px;
  position: fixed;
  bottom: 50px;
  right: 20px;
  z-index: 999;
  cursor: pointer;

  > img {
    width: 100%;
  }

  @include min-width(768px) {
    width: 121px;
    height: 139px;
    bottom: 100px;
    right: 100px;
  }

  .btn-hover {
    display: none;
  }

  @include min-width(1025px) {
    .btn-def {
    }

    .btn-hover {
      display: none;
      opacity: 0;
    }

    &:hover {
      .btn-def {
        display: none;
        opacity: 0;
      }
      .btn-hover {
        display: block;
        opacity: 1;
      }
    }
  }
}
</style>
