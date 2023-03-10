!<template>
  <div class="cd-popup2" role="alert">
    <div class="cd-popup-container">
			<div class="cd-main">
				<img src="@/assets/images/newpic/影像聲音後製.svg" />
			</div>
      <a
        href="javascript:;"
        class="cd-popup-close img-replace"
        >Close</a
      >
    </div>
  </div>
</template>

<script>
export default {
	mounted() {
    //open popup
    $(".cd-popup-trigger2").on("click", function (event) {
      event.preventDefault();
      $(".cd-popup2").addClass("is-visible");
    });

    //close popup
    $(".cd-popup2").on("click", function (event) {
      if (
        $(event.target).is(".cd-popup-close") ||
        $(event.target).is(".cd-popup2")
      ) {
        event.preventDefault();
        $(this).removeClass("is-visible");
      }
    });
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/mixin.scss";
@import "@/assets/scss/variables.scss";
@import "@/assets/scss/reset.scss";

// * ==========================================================================
// * popup  表單彈窗
// * ==========================================================================

.cd-popup2 {
  position: fixed;
  left: 0;
  top: 0;
  height: 100%;
  width: 100%;
  background-color: rgba(0, 0, 0, 0.4);
  opacity: 0;
  visibility: hidden;
  transition: opacity 0.3s 0s, visibility 0s 0.3s;
  z-index: 10001;
}
.cd-popup2.is-visible {
  display: flex;
  align-items: center;
  justify-content: center;
  opacity: 1;
  visibility: visible;
  transition: opacity 0.3s 0s, visibility 0s 0s;
}

.cd-popup-container {
  width: 350px;
  height: 546px;
  margin: 4em auto;
  border: 1px solid $color-black;
  background: $color-white;
  display: block;
  transition-property: transform;
  transition-duration: 0.3s;
	overflow: hidden;

  @include min-width(768px) {
    width: 550px;
  }

  @include min-width(1025px) {
    display: flex;
    position: relative;
    width: 90%;
    max-width: 1200px;
    height: 700px;
    text-align: center;
    transform: translateY(100%);
    -webkit-backface-visibility: hidden;
  }
}

.cd-main{
	height: 546px;
	padding: 1rem;
	overflow-y: auto;

	@include min-width(1025px) {
		height: 700px;
		padding: 3rem;
	}

	>img{
		width: 100%;
	}
}

//關閉X按鈕
.cd-popup-close {
  position: fixed;
  top: 31px;
  right: 28px;
  width: 30px;
  height: 30px;
  display: inline-block;
  overflow: hidden;
  text-indent: 100%;
  color: transparent;
  white-space: nowrap;
  z-index: 10;

  @include min-width(1025px) {
    top: 31px;
    right: 28px;
  }
}

.cd-popup-close::before,
.cd-popup-close::after {
  content: "";
  position: absolute;
  top: 12px;
  width: 29px;
  height: 2px;
  background-color: $color-primary-2;
}
.cd-popup-close {
  &::before {
    transform: rotate(45deg);
    left: 1px;
  }
}
.cd-popup-close {
  &::after {
    transform: rotate(-45deg);
    right: 1px;
  }
}

.is-visible .cd-popup-container {
  transform: translateY(0%);
}

.popup-swiper-form {
  overflow: hidden;
}
.swiper-pagination {
  bottom: -35px !important;

  .swiper-pagination-bullet {
    background-color: $color-white;
    border: 1px solid $color-primary-2;
    opacity: 1;

    &.swiper-pagination-bullet-active {
      background-color: $color-primary-2;
    }
  }
}
</style>