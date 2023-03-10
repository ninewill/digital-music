<template>
  <svg class="point-c">
    <circle id="ball" cx="0" cy="0" r="8" />
  </svg>
</template>

<script>
export default {
  components: {},
  mounted() {
    $(function () {
      const $window = $(window);

      if ($(window).width() < 767) {
        // 當視窗寬度小於767px時執行
      } else {
        // 當視窗寬度不小於767px時執行
        var ease = 0.1;
        var ball = $("#ball");
        var pos = { x: 0, y: 0 };
        var mouse = { x: 0, y: 0 };

        $(window).mousemove(function (e) {
          mouse.x = e.clientX;
          mouse.y = e.clientY;
        });

        TweenLite.ticker.addEventListener("tick", update);

        function update() {
          pos.x += (mouse.x - pos.x) * ease;
          pos.y += (mouse.y - pos.y) * ease;

          ball.attr("cx", pos.x);
          ball.attr("cy", pos.y);
        }

        $("a").hover(
          function () {
            TweenMax.to(ball, 0.2, { attr: { r: "50", ease: Power3.easeOut } });
          },
          function () {
            TweenMax.to(ball, 0.2, { attr: { r: "8", ease: Power3.easeOut } });
          }
        );
      }
    });
  },
};
</script>

<style lang="scss">
@import "@/assets/scss/mixin.scss";
@import "@/assets/scss/variables.scss";
@import "@/assets/scss/reset.scss";

.point-c {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  fill: $color-primary-1;
  pointer-events: none;
  z-index: 100000;
}

#ball {
  opacity: 0.8;
}
</style>