<template>
  <div>
    <div class="s-title s3-title">
      <h2 class="h2">STUDENT WORKS</h2>
    </div>
    <div class="s-content s3-content">
      <div class="s3-content-title"></div>
      <div class="s3-content-cards">
        <div class="card-list">
          <div class="card-list-nav">
            <div class="card-list-nav-title">PLAYLIST</div>
            <div class="nav-wrap nav-wrap-pc">
              <a @click="handChangePage(0)" :class="{ active: pageIdx === 0 }">
                <span>01</span>
                <div class="nav-menu">
                  <span>音樂製作人</span>
                  <span>POST PRODUCTION</span>
                  <div class="border-cube"></div>
                </div>
              </a>
              <a @click="handChangePage(1)" :class="{ active: pageIdx === 1 }">
                <span>02</span>
                <div class="nav-menu">
                  <span>職業歌唱</span>
                  <span>VOCALIST</span>
                  <div class="border-cube"></div>
                </div>
              </a>
              <a @click="handChangePage(2)" :class="{ active: pageIdx === 2 }">
                <span>03</span>
                <div class="nav-menu">
                  <span>歌詞創作</span>
                  <span>LYRICS CREATION</span>
                  <div class="border-cube"></div>
                </div>
              </a>
            </div>
            <div class="nav-wrap nav-wrap-mb">
              <a @click="handChangePage(0)" :class="{ active: pageIdx === 0 }">
                <div class="nav-menu">
                  <span>音樂製作人</span>
                </div>
              </a>
              <a @click="handChangePage(1)" :class="{ active: pageIdx === 1 }">
                <div class="nav-menu">
                  <span>職業歌唱</span>
                </div>
              </a>
              <a @click="handChangePage(2)" :class="{ active: pageIdx === 2 }">
                <div class="nav-menu">
                  <span>歌詞創作</span>
                </div>
              </a>
            </div>
          </div>
        </div>
        <div class="card-page">
          <div class="card-pages">
            <div class="page1" v-if="pageIdx === 0">
              <div class="mid">
                <div class="music-wrap">
                  <div class="music">
                    <div class="music-img">
                      <img
                        src="@/assets/images/pic/pic_06-2_music_1x.jpeg"
                        alt="圖片"
                      />
                    </div>
                    <audio controls>
                      <source
                        src="@/assets/images/music/學員作品/01_音樂製作人/01.mp3"
                        type="audio/mpeg"
                      />
                    </audio>
                    <div class="music-info">
                      <img
                        src="@/assets/images/pic/pic_06_text1-1.svg"
                        alt="圖片"
                      />
                    </div>
                  </div>
                  <div class="music">
                    <div class="music-img">
                      <img
                        src="@/assets/images/pic/pic_06-2_music_1x.jpeg"
                        alt="圖片"
                      />
                    </div>
                    <audio controls>
                      <source
                        src="@/assets/images/music/學員作品/01_音樂製作人/02.mp3"
                        type="audio/mpeg"
                      />
                    </audio>
                    <div class="music-info">
                      <img
                        src="@/assets/images/pic/pic_06_text1-2.svg"
                        alt="圖片"
                      />
                    </div>
                  </div>
                  <div class="music">
                    <div class="music-img">
                      <img
                        src="@/assets/images/pic/pic_06-2_music_1x.jpeg"
                        alt="圖片"
                      />
                    </div>
                    <audio controls>
                      <source
                        src="@/assets/images/music/學員作品/01_音樂製作人/03.mp3"
                        type="audio/mpeg"
                      />
                    </audio>
                    <div class="music-info">
                      <img
                        src="@/assets/images/pic/pic_06_text1-3.svg"
                        alt="圖片"
                      />
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class="page2" v-show="pageIdx === 1">
              <div class="mid">
                <div class="music-wrap">
                  <div class="music">
                    <div class="music-img">
                      <img
                        src="@/assets/images/pic/pic_06-2_music_1x.jpeg"
                        alt="圖片"
                      />
                    </div>
                    <audio controls>
                      <source
                        src="@/assets/images/music/學員作品/02_職業歌唱/01.mp3"
                        type="audio/mpeg"
                      />
                    </audio>
                    <div class="music-info">
                      <img
                        src="@/assets/images/pic/pic_06_text2-1.svg"
                        alt="圖片"
                      />
                    </div>
                  </div>
                  <div class="music">
                    <div class="music-img">
                      <img
                        src="@/assets/images/pic/pic_06-2_music_1x.jpeg"
                        alt="圖片"
                      />
                    </div>
                    <audio controls>
                      <source
                        src="@/assets/images/music/學員作品/02_職業歌唱/02.mp3"
                        type="audio/mpeg"
                      />
                    </audio>
                    <div class="music-info">
                      <img
                        src="@/assets/images/pic/pic_06_text2-2.svg"
                        alt="圖片"
                      />
                    </div>
                  </div>
                  <div class="music">
                    <div class="music-img">
                      <img
                        src="@/assets/images/pic/pic_06-2_music_1x.jpeg"
                        alt="圖片"
                      />
                    </div>
                    <audio controls>
                      <source
                        src="@/assets/images/music/學員作品/02_職業歌唱/03.mp3"
                        type="audio/mpeg"
                      />
                    </audio>
                    <div class="music-info">
                      <img
                        src="@/assets/images/pic/pic_06_text2-3.svg"
                        alt="圖片"
                      />
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class="page3" v-show="pageIdx === 2">
              <div class="mid">
                <div class="music-wrap">
                  <div class="music music-popup1">
                    <div class="music-img">
                      <img
                        src="@/assets/images/pic/pic_06-2_music_1x.jpeg"
                        alt="圖片"
                      />
                    </div>
                    <div class="music-info">
                      <img
                        src="@/assets/images/pic/pic_06_text3-1.svg"
                        alt="圖片"
                      />
                    </div>
                  </div>
                  <div class="music music-popup2">
                    <div class="music-img">
                      <img
                        src="@/assets/images/pic/pic_06-2_music_1x.jpeg"
                        alt="圖片"
                      />
                    </div>
                    <div class="music-info">
                      <img
                        src="@/assets/images/pic/pic_06_text3-2.svg"
                        alt="圖片"
                      />
                    </div>
                  </div>
                  <div class="music music-popup3">
                    <div class="music-img">
                      <img
                        src="@/assets/images/pic/pic_06-2_music_1x.jpeg"
                        alt="圖片"
                      />
                    </div>
                    <div class="music-info">
                      <img
                        src="@/assets/images/pic/pic_06_text3-3.svg"
                        alt="圖片"
                      />
                    </div>
                  </div>
                </div>
								<Music />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

import Music from "@/components/Music.vue";

export default {
	components: {
    Music,
  },
  data() {
    return {
      pageIdx: 0,
    };
  },
  methods: {
    handChangePage: function (idx) {
      this.pageIdx = idx;
    },
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/mixin.scss";
@import "@/assets/scss/variables.scss";
@import "@/assets/scss/reset.scss";

.s3-title {
  width: 335px;
  height: 30px;
  position: absolute;
  top: -6%;
  left: 50%;
  z-index: 1;
  margin-left: -167.5px;

  @include min-width(525px) {
    width: 478.8px;
    height: 43.2px;
    top: -5%;
    margin-left: -239.4px;
  }

  @include min-width(768px) {
    width: 638.4px;
    height: 57.6px;
    margin-left: -319.2px;
  }

  @include min-width(1025px) {
    width: 446px;
    height: 40px;
    top: -40%;
    margin-left: -223px;
  }

  @include min-width(1440px) {
    width: 558px;
    height: 50px;
    top: -30%;
    margin-left: -279px;
  }

  @include min-width(1920px) {
    width: 798px;
    height: 72px;
    margin-left: -399px;
  }

  .h2 {
    width: 100%;
    height: 100%;
    display: block;
    position: absolute;
    top: 0px;
    left: 0px;
    background: url("@/assets/images/pic/pic_06_STUDENTWORKS.svg") no-repeat
      center/contain;
    @include hidetext;
  }
}

.s3-content {
  position: relative;
  width: 100%;
  border: 5px solid transparent;
  border-radius: 25px;
  background-image: linear-gradient($color-black, $color-black),
    linear-gradient(to right, #fff176, #00e0b8);
  background-origin: border-box;
  background-clip: content-box, border-box;

  &::after {
    content: "";
    width: 97px;
    height: 204.8px;
    display: block;
    position: absolute;
    bottom: -70px;
    right: 0px;
    background: url("@/assets/images/pic/pic_06-1_people.svg") no-repeat
      center/contain;

    @include min-width(768px) {
      width: 164.8px;
      height: 346.4px;
      right: -30px;
			bottom: 0;
    }

    @include min-width(1025px) {
      width: 144.2px;
      height: 303.1px;
      top: -130px;
      right: -60px;
      bottom: auto;
    }

    @include min-width(1440px) {
      width: 206px;
      height: 433px;
      right: -100px;
    }
  }

  .s3-content-title {
    position: absolute;
    top: 0;
    margin-top: -18%;
    margin-left: 0;
    width: 100%;
    padding-bottom: 29.32%;
    background: url("@/assets/images/pic/mobile/pic_06_title06.svg") no-repeat;
    background-size: contain;
    background-position: 50% 50%;

    @include min-width(768px) {
      margin-left: 25%;
      width: 50%;
      padding-bottom: 17.32%;
      margin-top: -10%;
    }

    @include min-width(850px) {
      margin-left: 23%;
    }

    @include min-width(1025px) {
      margin-top: -7%;
      margin-left: 1.5rem;
      padding-bottom: 12.85%;
      background: url("@/assets/images/pic/pic_06_title.svg") no-repeat;
      background-size: contain;
      background-position: 0 100%;
    }
  }
}

.s3-content-cards {
  padding: 5rem 2rem;

  @include min-width(768px) {
    padding: 8rem 5rem;
  }

  @include min-width(1025px) {
    padding: 6rem 5rem;
    display: flex;
    justify-content: space-between;
  }

  @include min-width(1440px) {
    padding: 8rem 5rem;
		padding-bottom: 3rem;
  }

  .card-list {
    width: 100%;

    @include min-width(1025px) {
      width: 25%;
    }

    @include min-width(1440px) {
      width: 20%;
    }

    @include min-width(1920px) {
      width: 17%;
    }

    .card-list-nav {
      .card-list-nav-title {
        text-align: center;
        font-size: 36px;
        background: linear-gradient(137.1deg, #fff176 14.56%, #00e0b8 85.34%);
        background-clip: text;
        color: transparent;

        @include min-width(1025px) {
          text-align: left;
          font-size: 30px;
        }

        @include min-width(1440px) {
          font-size: 36px;
        }
      }

      .nav-wrap {
        > a {
          display: block;
          cursor: pointer;
          margin-top: 1.5rem;

          > span {
            display: block;
            color: $color-primary-1;
          }

          .nav-menu {
            position: relative;
            margin-top: 0.25rem;

            > span {
              display: block;
              color: $color-white;
              font-size: 12px;
              opacity: 0.5;

              @include min-width(768px) {
                font-size: 16px;
              }

              @include min-width(1025px) {
                font-size: 14px;
                line-height: 20px;
              }

              @include min-width(1440px) {
                font-size: 16px;
                line-height: 27px;
              }
            }

            .border-cube {
              width: 20px;
              height: 20px;
              position: absolute;
              right: 0;
              bottom: 0;
              border-right: 1px solid $color-primary-1;
              border-bottom: 1px solid $color-primary-1;
            }
          }

          &.active {
            .nav-menu {
              position: relative;

              &:before {
                content: "";
                position: absolute;
                left: -25px;
                top: 50%;
                margin-top: -7px;
                width: 12px;
                height: 14px;
                display: block;
                background: url("@/assets/images/pic/pic_06_arrow.svg")
                  no-repeat center/contain;
              }

              > span {
                opacity: 1;
              }
            }
          }
        }

        &.nav-wrap-pc {
          display: none;

          @include min-width(1025px) {
            display: block;
          }
        }

        &.nav-wrap-mb {
          width: 100%;
          margin: 0 auto;
          margin-top: 2rem;
          display: flex;
          align-items: center;
          border: 1px solid $color-primary-1;

          > a {
            width: 33.33%;
            padding: 5px;
            margin-top: 0;
            text-align: center;
            border-right: 1px solid $color-primary-1;

            @include min-width(768px) {
              padding: 10px;
            }

            &:last-child {
              border-right: none;
            }

            .nav-menu {
              margin-top: 0;

              > span {
                opacity: 1;
                color: $color-primary-1;
              }
            }

            &.active {
              background-color: $color-primary-1;

              .nav-menu {
                margin-top: 0;
                position: relative;

                > span {
                  color: $color-white;
                }

                &:before {
                  display: none;
                }
              }
            }

            > span {
              text-align: center;
              opacity: 1;
            }
          }

          @include min-width(1025px) {
            display: none;
          }
        }
      }
    }
  }

  .card-page {
    width: 100%;

    @include min-width(1025px) {
      width: 68%;
    }

    @include min-width(1440px) {
      width: 77%;
    }

    @include min-width(1920px) {
      width: 80%;
    }

    .music-wrap {
      margin-top: 2rem;

      @include min-width(1025px) {
        margin-top: 0;
        display: flex;
        justify-content: space-between;
      }

      .music-wrap-left {
        width: 50%;

        > video {
          width: 100%;
        }
      }

      .music-wrap-right {
        width: 50%;
        display: flex;
        align-items: center;
        justify-content: center;

        .music-wrap-right-img {
          display: flex;

          > img {
            margin: 0 auto;
          }
        }
      }
    }

    .music {
      width: 100%;
      margin-bottom: 2rem;
			cursor: pointer;

      @include min-width(1025px) {
        width: 30%;
        margin-bottom: 0;
      }

      .music-img {
        > img {
          width: 100%;
        }
      }

      audio {
        margin-top: 1.5rem;
        width: 100%;

        @include min-width(1025px) {
          height: 40px;
        }
      }

      .music-info {
        margin-top: 1rem;

        > img {
          width: 100%;
        }
      }
    }
  }
}
</style>