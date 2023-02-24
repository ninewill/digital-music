<template>
  <div id="wrapper" class="layout">
    <Navbar />
    <Menu />
    <router-view />
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from "@/components/Navbar.vue";
import Menu from "@/components/Menu.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "HomeView",
  components: {
    Navbar,
    Menu,
    Footer,
  },
  mounted() {
    /*
     * ==========================================================================
     * MENU 設計
     * ==========================================================================
     */

    var menuBox = $(".menu-page");
    var menuBg = $(".menu-page-left__bg");
    var menuMic = $(".mic-icon");
    var menuTitle = $(".menu-title");
    var menuList1 = $(".menu-inner-list1");
    var menuList2 = $(".menu-inner-list2");
    var menuList3 = $(".menu-inner-list3");
    var menuWrap = $(".menu-btn a");
    var open = false;
    var tl = new TimelineMax();
    tl.pause();
    tl.fromTo(
      menuBox,
      0.4,
      {
        x: "-100%",
        opacity: 0,
      },
      { x: 0, opacity: 1, ease: Power4.easeInOut }
    );

    tl.staggerFrom(menuBg, 0.2, { autoAlpha: 0, y: -15 });
    tl.staggerFrom(menuMic, 0.15, { autoAlpha: 0, y: 15 });
    tl.staggerFrom(menuTitle, 0.15, { autoAlpha: 0, y: 15 });
    tl.staggerFrom(menuList1, 0.2, { autoAlpha: 0, y: 15 });
    tl.staggerFrom(menuList2, 0.2, { autoAlpha: 0, y: 15 });
    tl.staggerFrom(menuList3, 0.2, { autoAlpha: 0, y: 15 });

    /*
     * ==========================================================================
     * MENU 設計
     * ==========================================================================
     */
    menuWrap.on("click", () => {
      if (open === false) {
        tl.play();
        $("body,html").addClass("over-hidden");
      }
      if (open === true) {
        tl.reverse();
        $("body,html").removeClass("over-hidden");
      }
      open = !open;
    });

    $(".c-link").click(function () {
      let target = this.hash,
        $target = $(target).offset().top;

      $("html, body").animate({ scrollTop: $target }), 1500;

      if (open === false) {
        tl.play();
        $("body,html").addClass("over-hidden");
      }
      if (open === true) {
        tl.reverse();
        $("body,html").removeClass("over-hidden");
      }
      open = !open;
    });
  },
};
</script>

<style lang="scss">
@import "@/assets/scss/mixin.scss";
@import "@/assets/scss/variables.scss";
@import "@/assets/scss/reset.scss";

html,
body {
  width: 100%;
  font-size: map-get($fontsize, 5);
}

body {
  line-height: 1.6em;
  overflow-y: auto;
  overflow-x: hidden;
  position: relative;
  font-size: 1rem;
  font-family: "微軟正黑體", "Microsoft JhengHei", sans-serif, Arial, Helvetica;
  letter-spacing: 0.5px;
  background-color: $color-black;
}

// * ==========================================================================
// * 主要內容區域（#main 裡面的基本樣式）
// * ==========================================================================

.over-hidden {
  overflow: hidden;
}

#main {
  //padding-top: 85px;
  padding-bottom: 85px;
  position: relative;

  @include min-width(1025px) {
    //padding-top: 90px;
    padding-bottom: 150px;
  }
}

// * ==========================================================================
// * 頁面外圍控制整體布局寬度
// * ==========================================================================

.wrap {
  margin: 0 auto;
}

.wrap-content {
  transition: 0.2s;
}
</style>
