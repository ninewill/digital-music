<template>
  <div class="tc-bar-wrap">
    <div class="tc-info">
      <div class="h3">Nuendo 全台唯一德國原廠授權認證教育中心</div>
      <p>
        2022年赫綵設計學院獨家搶先獲得
        德國Steinberg原廠認證ATC，接軌業界專業升級。
      </p>
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

.tc-bar-wrap {
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;

  .tc-info {
		position: relative;
		margin-left: -15%;
    > .h3 {
      font-size: 2vw;
      color: $color-primary-1;
    }
    > p {
      margin-top: 1rem;
      font-size: 1.2vw;
      color: $color-white;
    }

    &::before {
      content: "";
			position: absolute;
			top: 0;
			left: -100px;
      display: block;
			width: 90px;
			height: 90px;
      background: url("@/assets/images/newpic/s5_star.png") no-repeat;
      background-size: contain;
      background-position: 50% 50%;
    }

    &::after {
      content: "";
			position: absolute;
			top: 50%;
			right: -300px;
			margin-top: -152.5px;
      display: block;
			width: 215px;
			height: 305px;
      background: url("@/assets/images/newpic/s5_license.jpg") no-repeat;
      background-size: contain;
      background-position: 50% 50%;
    }
  }
}
</style>