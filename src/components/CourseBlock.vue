<template>
  <div class="course-area">
    <div class="s-title s2-title">
      <div class="s2-title-left">
        <div class="s2-title-left-l">
					<img src="@/assets/images/newpic/s4_part1.png" alt="圖片" />
				</div>
				<div class="s2-title-left-r">
					<div class="h3">Mixcraft 輕鬆快速上手</div>
					<p>輕鬆入門、快速上手，還有取之不盡的強大素材庫！</p>
				</div>
      </div>
      <div class="s2-title-right">
        <img src="@/assets/images/newpic/s4_p1hour.png" alt="圖片" />
      </div>
    </div>
    <!--COURSE Card-->
    <div class="s-content s2-content"></div>
  </div>
</template>

<script>
</script>

<style lang="scss" scoped>
@import "@/assets/scss/mixin.scss";
@import "@/assets/scss/variables.scss";
@import "@/assets/scss/reset.scss";

.course-area {
  position: relative;
}

.s2-title{
	display: flex;
	align-items: center;
	justify-content: space-between;

	.s2-title-left{
		width: 60%;
		display: flex;

		.s2-title-left-l{
			width: 25%;

			>img{
				width: 100%;
			}
		}

		.s2-title-left-r{
			width: 70%;
			display: flex;
			flex-direction: column;
			align-items: flex-start;
			justify-content: center;

			>img{
				width: 100%;
			}

			.h3{
				font-weight: 700;
				font-size: 32px;
				line-height: 46px;
				color: $color-primary-1;
			}

			p{
				margin-top: 1rem;
				font-weight: 350;
				font-size: 20px;
				color: $color-white;
			}
		}
	}

	.s2-title-right{
		width: 30%;

		>img{
				width: 100%;
			}
	}
}
</style>