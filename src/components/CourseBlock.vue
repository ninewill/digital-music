<template>
  <div class="course-area">
    <div class="s-title s2-title">
      <h2 class="h2">COURSE</h2>
    </div>
    <!--COURSE Card-->
    <div class="s-content s2-content">
      <div class="s2-content-cards">
        <div class="card-left card-list">
          <div class="card-tags">
            <div class="level level1">Level.01</div>
            <div class="level level2">Level.02</div>
            <div class="level level3">Level.03</div>
          </div>
          <div class="card-list-nav">
            <a @click="handChangePage(0)" :class="{ active: pageIdx === 0 }">
              <span>音樂製作人</span>
              <span>音樂概論/詞曲創作/歌唱技巧/數位編曲</span>
            </a>
            <a @click="handChangePage(1)" :class="{ active: pageIdx === 1 }">
              <span>詞曲創作</span>
              <span>聽力訓練/填詞技巧/作曲實務/DEMO錄音</span>
            </a>
            <a @click="handChangePage(2)" :class="{ active: pageIdx === 2 }">
              <span>編曲配樂</span>
              <span>樂譜識譜/配器編曲/效果器外掛/混音技法</span>
            </a>
            <a @click="handChangePage(3)" :class="{ active: pageIdx === 3 }">
              <span>錄音室職業歌唱</span>
              <span>發聲呼吸/共鳴咬字/歌唱健診/和聲樂理</span>
            </a>
            <a @click="handChangePage(4)" :class="{ active: pageIdx === 4 }">
              <span>EDM電音製作</span>
              <span>介紹器材/實用樂理/樂曲結構/素材混音</span>
            </a>
            <a @click="handChangePage(5)" :class="{ active: pageIdx === 5 }">
              <span>錄音及混音技術</span>
              <span>音樂格式/混音實作/人聲錄製/樂器錄製</span>
            </a>
            <a @click="handChangePage(6)" :class="{ active: pageIdx === 6 }">
              <span>影視配樂作曲</span>
              <span>術語解釋/配樂解析/影像解讀/過帶混音</span>
            </a>
            <a @click="handChangePage(7)" :class="{ active: pageIdx === 7 }">
              <span>電影動畫配樂創作</span>
              <span>音樂概論/和弦記憶法/作曲風格/創作實務</span>
            </a>
          </div>
        </div>
        <div class="card-right card-page">
          <div class="card-lines">
            <span></span>
            <span></span>
            <span></span>
          </div>
          <div id="course" class="card-pages">
            <div class="page1" v-show="pageIdx === 0">
              <div class="mid">
                <div class="mid-title">
                  <div class="mid-title__left">
                    <div class="mid-title__left-t">
                      <div class="mid-title__left-img">
                        <img
                          src="@/assets/images/pic/pic_03_DigitalMusic.svg"
                          alt="圖片"
                        />
                      </div>
                      <span>音樂製作人</span>
                    </div>
                    <div class="mid-title__left-b">
                      72小時晉升音樂製作人，別再當錄音室助理！
                    </div>
                  </div>
                  <div class="mid-title__right">
                    <span>必學課程</span>
                    <span>72HRS</span>
                  </div>
                </div>
                <div class="mid-item">
                  <ul>
                    <li>了解市場</li>
                    <li>樂理概念</li>
                    <li>填詞技巧</li>
                    <li>作曲手法</li>
                    <li>配樂編曲</li>
                    <li>出版引薦</li>
                    <li>版權概念</li>
                    <li>混音實務</li>
                    <li>流行歌唱</li>
                    <li>錄音實戰</li>
                  </ul>
                  <div class="mid-music">
                    <div class="mid-music-title">
                      <div class="mid-music-title__left">
                        <img
                          src="@/assets/images/pic/pic_03_career.svg"
                          alt="圖片"
                        />
                      </div>
                      <p>音樂製作人 / 詞曲創作人 / 出版歌手</p>
                    </div>
                    <div class="music-wrap">
                      <div class="music">
                        <div class="music-img">
                          <img
                            src="@/assets/images/pic/pic_03_music01_1x.jpeg"
                            alt="圖片"
                          />
                        </div>
                        <audio controls>
                          <source
                            src="@/assets/images/music/課程講師作品/01_音樂製作人/01.mp3"
                            type="audio/mpeg"
                          />
                        </audio>
                        <div class="music-info">
                          <img
                            src="@/assets/images/pic/pic_03_text1-1.svg"
                            alt="圖片"
                          />
                        </div>
                      </div>
                      <div class="music">
                        <div class="music-img">
                          <img
                            src="@/assets/images/pic/pic_03_music01_1x.jpeg"
                            alt="圖片"
                          />
                        </div>
                        <audio controls>
                          <source
                            src="@/assets/images/music/課程講師作品/01_音樂製作人/02.mp3"
                            type="audio/mpeg"
                          />
                        </audio>
                        <div class="music-info">
                          <img
                            src="@/assets/images/pic/pic_03_text1-2.svg"
                            alt="圖片"
                          />
                        </div>
                      </div>
                      <div class="music">
                        <div class="music-img">
                          <img
                            src="@/assets/images/pic/pic_03_music01_1x.jpeg"
                            alt="圖片"
                          />
                        </div>
                        <audio controls>
                          <source
                            src="@/assets/images/music/課程講師作品/01_音樂製作人/03.mp3"
                            type="audio/mpeg"
                          />
                        </audio>
                        <div class="music-info">
                          <img
                            src="@/assets/images/pic/pic_03_text1-3.svg"
                            alt="圖片"
                          />
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
              <div class="course-btn">
                <a class="cd-popup-trigger0" href="javascript:;"
                  >觀看完整課綱</a
                >
              </div>
            </div>
            <div class="page2" v-show="pageIdx === 1">
              <div class="mid">
                <div class="mid-title">
                  <div class="mid-title__left">
                    <div class="mid-title__left-t">
                      <div class="mid-title__left-img">
                        <img
                          src="@/assets/images/pic/pic_03_DigitalMusic.svg"
                          alt="圖片"
                        />
                      </div>
                      <span>詞曲創作</span>
                    </div>
                    <div class="mid-title__left-b">
                      邏輯思考撰寫詞曲，讓你創作不卡頓！
                    </div>
                  </div>
                  <div class="mid-title__right">
                    <span>必學課程</span>
                    <span>48HRS</span>
                  </div>
                </div>
                <div class="mid-item">
                  <ul>
                    <li>樂譜運用</li>
                    <li>了解產業</li>
                    <li>跨語言填詞</li>
                    <li>版權概念</li>
                    <li>創作實務</li>
                    <li>出版引薦</li>
                    <li>DEMO錄製</li>
                    <li>作曲伴奏</li>
                    <li>賣歌比稿</li>
                    <li>調性樂理</li>
                  </ul>
                  <div class="mid-music">
                    <div class="mid-music-title">
                      <div class="mid-music-title__left">
                        <img
                          src="@/assets/images/pic/pic_03_career.svg"
                          alt="圖片"
                        />
                      </div>
                      <p>職業詞曲創作人 / 音樂老師</p>
                    </div>
                    <div class="music-wrap">
                      <div class="music">
                        <div class="music-img">
                          <img
                            src="@/assets/images/pic/pic_03_music01_1x.jpeg"
                            alt="圖片"
                          />
                        </div>
                        <audio controls>
                          <source
                            src="@/assets/images/music/課程講師作品/02_詞曲創作/01.mp3"
                            type="audio/mpeg"
                          />
                        </audio>
                        <div class="music-info">
                          <img
                            src="@/assets/images/pic/pic_03_text2-1.svg"
                            alt="圖片"
                          />
                        </div>
                      </div>
                      <div class="music">
                        <div class="music-img">
                          <img
                            src="@/assets/images/pic/pic_03_music01_1x.jpeg"
                            alt="圖片"
                          />
                        </div>
                        <audio controls>
                          <source
                            src="@/assets/images/music/課程講師作品/02_詞曲創作/02.mp3"
                            type="audio/mpeg"
                          />
                        </audio>
                        <div class="music-info">
                          <img
                            src="@/assets/images/pic/pic_03_text2-2.svg"
                            alt="圖片"
                          />
                        </div>
                      </div>
                      <div class="music">
                        <div class="music-img">
                          <img
                            src="@/assets/images/pic/pic_03_music01_1x.jpeg"
                            alt="圖片"
                          />
                        </div>
                        <audio controls>
                          <source
                            src="@/assets/images/music/課程講師作品/02_詞曲創作/03.mp3"
                            type="audio/mpeg"
                          />
                        </audio>
                        <div class="music-info">
                          <img
                            src="@/assets/images/pic/pic_03_text2-3.svg"
                            alt="圖片"
                          />
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
              <div class="course-btn">
                <a class="cd-popup-trigger2" href="javascript:;"
                  >觀看完整課綱</a
                >
              </div>
            </div>
            <div class="page3" v-show="pageIdx === 2">
              <div class="mid">
                <div class="mid-title">
                  <div class="mid-title__left">
                    <div class="mid-title__left-t">
                      <div class="mid-title__left-img">
                        <img
                          src="@/assets/images/pic/pic_03_DigitalMusic.svg"
                          alt="圖片"
                        />
                      </div>
                      <span>編曲配樂</span>
                    </div>
                    <div class="mid-title__left-b">
                      術業有專攻，音樂大師團隊傳授技能
                    </div>
                  </div>
                  <div class="mid-title__right">
                    <span>必學課程</span>
                    <span>48HRS</span>
                  </div>
                </div>
                <div class="mid-item">
                  <ul>
                    <li>視譜學習</li>
                    <li>軟硬體概念</li>
                    <li>配器編曲</li>
                    <li>和聲解析</li>
                    <li>音箱效果器</li>
                    <li>出版引薦</li>
                    <li>分軌混音</li>
                    <li>DEMO製作</li>
                    <li>影像配樂</li>
                    <li>弦樂配置</li>
                  </ul>
                  <div class="mid-music">
                    <div class="mid-music-title">
                      <div class="mid-music-title__left">
                        <img
                          src="@/assets/images/pic/pic_03_career.svg"
                          alt="圖片"
                        />
                      </div>
                      <p>音樂製作人 / 詞曲創作人 / 出版歌手</p>
                    </div>
                    <div class="music-wrap">
                      <div class="music">
                        <div class="music-img">
                          <img
                            src="@/assets/images/pic/pic_03_music01_1x.jpeg"
                            alt="圖片"
                          />
                        </div>
                        <audio controls>
                          <source
                            src="@/assets/images/music/課程講師作品/03_編曲配樂/01.mp3"
                            type="audio/mpeg"
                          />
                        </audio>
                        <div class="music-info">
                          <img
                            src="@/assets/images/pic/pic_03_text3-1.svg"
                            alt="圖片"
                          />
                        </div>
                      </div>
                      <div class="music">
                        <div class="music-img">
                          <img
                            src="@/assets/images/pic/pic_03_music01_1x.jpeg"
                            alt="圖片"
                          />
                        </div>
                        <audio controls>
                          <source
                            src="@/assets/images/music/課程講師作品/03_編曲配樂/02.mp3"
                            type="audio/mpeg"
                          />
                        </audio>
                        <div class="music-info">
                          <img
                            src="@/assets/images/pic/pic_03_text3-2.svg"
                            alt="圖片"
                          />
                        </div>
                      </div>
                      <div class="music">
                        <div class="music-img">
                          <img
                            src="@/assets/images/pic/pic_03_music01_1x.jpeg"
                            alt="圖片"
                          />
                        </div>
                        <audio controls>
                          <source
                            src="@/assets/images/music/課程講師作品/03_編曲配樂/03.mp3"
                            type="audio/mpeg"
                          />
                        </audio>
                        <div class="music-info">
                          <img
                            src="@/assets/images/pic/pic_03_text3-3.svg"
                            alt="圖片"
                          />
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
              <div class="course-btn">
                <a class="cd-popup-trigger3" href="javascript:;"
                  >觀看完整課綱</a
                >
              </div>
            </div>
            <div class="page4" v-show="pageIdx === 3">
              <div class="mid">
                <div class="mid-title">
                  <div class="mid-title__left">
                    <div class="mid-title__left-t">
                      <div class="mid-title__left-img">
                        <img
                          src="@/assets/images/pic/pic_03_DigitalMusic.svg"
                          alt="圖片"
                        />
                      </div>
                      <span>錄音室職業歌唱</span>
                    </div>
                    <div class="mid-title__left-b">
                      循序漸進系統化教學，專業引導教唱技巧！
                    </div>
                  </div>
                  <div class="mid-title__right">
                    <span>必學課程</span>
                    <span>48HRS</span>
                  </div>
                </div>
                <div class="mid-item">
                  <ul>
                    <li>樂譜介紹</li>
                    <li>呼吸法運用</li>
                    <li>發聲練習</li>
                    <li>聽力訓練</li>
                    <li>歌曲剖析</li>
                    <li>演唱競賽</li>
                    <li>對唱模擬</li>
                    <li>歌唱健檢</li>
                    <li>配唱實務</li>
                    <li>鼻音共鳴</li>
                  </ul>
                  <div class="mid-music">
                    <div class="mid-music-title">
                      <div class="mid-music-title__left">
                        <img
                          src="@/assets/images/pic/pic_03_career.svg"
                          alt="圖片"
                        />
                      </div>
                      <p>職業編曲配樂師 / 音樂老師 / 職業歌手 / 駐唱歌手</p>
                    </div>
                    <div class="music-wrap">
                      <div class="music-wrap-left">
                        <video class="" autoplay muted loop controls>
                          <source
                            src="@/assets/images/music/課程講師作品/04_錄音室職業歌唱/職業歌唱.mp4"
                            type="video/mp4"
                          />
                        </video>
                      </div>
                      <div class="music-wrap-right">
                        <div class="music-wrap-right-img">
                          <img
                            src="@/assets/images/pic/pic_03_text4-1.svg"
                            alt="圖片"
                          />
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
              <div class="course-btn">
                <a class="cd-popup-trigger4" href="javascript:;"
                  >觀看完整課綱</a
                >
              </div>
            </div>
            <div class="page5" v-show="pageIdx === 4">
              <div class="mid">
                <div class="mid-title">
                  <div class="mid-title__left">
                    <div class="mid-title__left-t">
                      <div class="mid-title__left-img">
                        <img
                          src="@/assets/images/pic/pic_03_DigitalMusic.svg"
                          alt="圖片"
                        />
                      </div>
                      <span>EDM電音製作</span>
                    </div>
                    <div class="mid-title__left-b">
                      電音製作全攻略，實戰經驗不可少！
                    </div>
                  </div>
                  <div class="mid-title__right">
                    <span>必學課程</span>
                    <span>72HRS</span>
                  </div>
                </div>
                <div class="mid-item">
                  <ul>
                    <li>EDM種類</li>
                    <li>操作架構</li>
                    <li>理解五線譜</li>
                    <li>配器講解</li>
                    <li>製作EQ表</li>
                    <li>母帶製作</li>
                    <li>Drop擴展</li>
                    <li>空間係效果</li>
                    <li>進階編曲</li>
                    <li>認識效果器</li>
                  </ul>
                  <div class="mid-music">
                    <div class="mid-music-title">
                      <div class="mid-music-title__left">
                        <img
                          src="@/assets/images/pic/pic_03_career.svg"
                          alt="圖片"
                        />
                      </div>
                      <p>音樂製作人 / 詞曲創作人 / 出版歌手</p>
                    </div>
                    <div class="music-wrap">
                      <div class="music">
                        <div class="music-img">
                          <img
                            src="@/assets/images/pic/pic_03_music01_1x.jpeg"
                            alt="圖片"
                          />
                        </div>
                        <audio controls>
                          <source
                            src="@/assets/images/music/課程講師作品/05_EDM電音製作/01.mp3"
                            type="audio/mpeg"
                          />
                        </audio>
                        <div class="music-info">
                          <img
                            src="@/assets/images/pic/pic_03_text5-1.svg"
                            alt="圖片"
                          />
                        </div>
                      </div>
                      <div class="music">
                        <div class="music-img">
                          <img
                            src="@/assets/images/pic/pic_03_music01_1x.jpeg"
                            alt="圖片"
                          />
                        </div>
                        <audio controls>
                          <source
                            src="@/assets/images/music/課程講師作品/05_EDM電音製作/02.wav"
                            type="audio/mpeg"
                          />
                        </audio>
                        <div class="music-info">
                          <img
                            src="@/assets/images/pic/pic_03_text5-2.svg"
                            alt="圖片"
                          />
                        </div>
                      </div>
                      <div class="music">
                        <div class="music-img">
                          <img
                            src="@/assets/images/pic/pic_03_music01_1x.jpeg"
                            alt="圖片"
                          />
                        </div>
                        <audio controls>
                          <source
                            src="@/assets/images/music/課程講師作品/05_EDM電音製作/03.mp3"
                            type="audio/mpeg"
                          />
                        </audio>
                        <div class="music-info">
                          <img
                            src="@/assets/images/pic/pic_03_text5-3.svg"
                            alt="圖片"
                          />
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
              <div class="course-btn">
                <a class="cd-popup-trigger5" href="javascript:;"
                  >觀看完整課綱</a
                >
              </div>
            </div>
            <div class="page6" v-show="pageIdx === 5">
              <div class="mid">
                <div class="mid-title">
                  <div class="mid-title__left">
                    <div class="mid-title__left-t">
                      <div class="mid-title__left-img">
                        <img
                          src="@/assets/images/pic/pic_03_DigitalMusic.svg"
                          alt="圖片"
                        />
                      </div>
                      <span>錄音及混音技術</span>
                    </div>
                    <div class="mid-title__left-b">
                      擺脫助理稱號，晉升全能錄音師及混音師
                    </div>
                  </div>
                  <div class="mid-title__right">
                    <span>必學課程</span>
                    <span>48HRS</span>
                  </div>
                </div>
                <div class="mid-item">
                  <ul>
                    <li>音樂格式</li>
                    <li>效果器理論</li>
                    <li>混音架構</li>
                    <li>軌道音準</li>
                    <li>精細剪輯</li>
                    <li>版權概念</li>
                    <li>樂器錄音</li>
                    <li>人聲錄音</li>
                    <li>線材原理</li>
                    <li>音響概論</li>
                  </ul>
                  <div class="mid-music">
                    <div class="mid-music-title">
                      <div class="mid-music-title__left">
                        <img
                          src="@/assets/images/pic/pic_03_career.svg"
                          alt="圖片"
                        />
                      </div>
                      <p>DJ唱片騎士 / 錄音師 / 混音師</p>
                    </div>
                    <div class="music-wrap">
                      <div class="music">
                        <div class="music-img">
                          <img
                            src="@/assets/images/pic/pic_03_music01_1x.jpeg"
                            alt="圖片"
                          />
                        </div>
                        <audio controls>
                          <source
                            src="@/assets/images/music/課程講師作品/06_錄音及混音技術/01.mp3"
                            type="audio/mpeg"
                          />
                        </audio>
                        <div class="music-info">
                          <img
                            src="@/assets/images/pic/pic_03_text6-1.svg"
                            alt="圖片"
                          />
                        </div>
                      </div>
                      <div class="music">
                        <div class="music-img">
                          <img
                            src="@/assets/images/pic/pic_03_music01_1x.jpeg"
                            alt="圖片"
                          />
                        </div>
                        <audio controls>
                          <source
                            src="@/assets/images/music/課程講師作品/06_錄音及混音技術/02.mp3"
                            type="audio/mpeg"
                          />
                        </audio>
                        <div class="music-info">
                          <img
                            src="@/assets/images/pic/pic_03_text6-2.svg"
                            alt="圖片"
                          />
                        </div>
                      </div>
                      <div class="music">
                        <div class="music-img">
                          <img
                            src="@/assets/images/pic/pic_03_music01_1x.jpeg"
                            alt="圖片"
                          />
                        </div>
                        <audio controls>
                          <source
                            src="@/assets/images/music/課程講師作品/06_錄音及混音技術/03.mp3"
                            type="audio/mpeg"
                          />
                        </audio>
                        <div class="music-info">
                          <img
                            src="@/assets/images/pic/pic_03_text6-3.svg"
                            alt="圖片"
                          />
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
              <div class="course-btn">
                <a class="cd-popup-trigger6" href="javascript:;"
                  >觀看完整課綱</a
                >
              </div>
            </div>
            <div class="page7" v-show="pageIdx === 6">
              <div class="mid">
                <div class="mid-title">
                  <div class="mid-title__left">
                    <div class="mid-title__left-t">
                      <div class="mid-title__left-img">
                        <img
                          src="@/assets/images/pic/pic_03_DigitalMusic.svg"
                          alt="圖片"
                        />
                      </div>
                      <span>影視配樂作曲</span>
                    </div>
                    <div class="mid-title__left-b">
                      視覺與聽覺的結合衝擊，爆發全新感受
                    </div>
                  </div>
                  <div class="mid-title__right">
                    <span>必學課程</span>
                    <span>72HRS</span>
                  </div>
                </div>
                <div class="mid-item">
                  <ul>
                    <li>基本術語</li>
                    <li>影像與旋律</li>
                    <li>配器解析</li>
                    <li>編寫實作</li>
                    <li>配樂案例</li>
                    <li>提案技巧</li>
                    <li>過帶混音</li>
                    <li>影視配樂</li>
                    <li>合成器分析</li>
                    <li>樂器擬真</li>
                  </ul>
                  <div class="mid-music">
                    <div class="mid-music-title">
                      <div class="mid-music-title__left">
                        <img
                          src="@/assets/images/pic/pic_03_career.svg"
                          alt="圖片"
                        />
                      </div>
                      <p>廣告配樂 / 電視配樂 / 配樂創作</p>
                    </div>
                    <div class="music-wrap">
                      <div class="music">
                        <div class="music-img">
                          <img
                            src="@/assets/images/pic/pic_03_music01_1x.jpeg"
                            alt="圖片"
                          />
                        </div>
                        <audio controls>
                          <source
                            src="@/assets/images/music/課程講師作品/07_影視配樂作曲/01.mp3"
                            type="audio/mpeg"
                          />
                        </audio>
                        <div class="music-info">
                          <img
                            src="@/assets/images/pic/pic_03_text7-1.svg"
                            alt="圖片"
                          />
                        </div>
                      </div>
                      <div class="music">
                        <div class="music-img">
                          <img
                            src="@/assets/images/pic/pic_03_music01_1x.jpeg"
                            alt="圖片"
                          />
                        </div>
                        <audio controls>
                          <source
                            src="@/assets/images/music/課程講師作品/07_影視配樂作曲/02.mp3"
                            type="audio/mpeg"
                          />
                        </audio>
                        <div class="music-info">
                          <img
                            src="@/assets/images/pic/pic_03_text7-2.svg"
                            alt="圖片"
                          />
                        </div>
                      </div>
                      <div class="music">
                        <div class="music-img">
                          <img
                            src="@/assets/images/pic/pic_03_music01_1x.jpeg"
                            alt="圖片"
                          />
                        </div>
                        <audio controls>
                          <source
                            src="@/assets/images/music/課程講師作品/07_影視配樂作曲/03.mp3"
                            type="audio/mpeg"
                          />
                        </audio>
                        <div class="music-info">
                          <img
                            src="@/assets/images/pic/pic_03_text7-3.svg"
                            alt="圖片"
                          />
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
              <div class="course-btn">
                <a class="cd-popup-trigger7" href="javascript:;"
                  >觀看完整課綱</a
                >
              </div>
            </div>
            <div class="page8" v-show="pageIdx === 7">
              <div class="mid">
                <div class="mid-title">
                  <div class="mid-title__left">
                    <div class="mid-title__left-t">
                      <div class="mid-title__left-img">
                        <img
                          src="@/assets/images/pic/pic_03_DigitalMusic.svg"
                          alt="圖片"
                        />
                      </div>
                      <span>電影動畫配樂創作</span>
                    </div>
                    <div class="mid-title__left-b">
                      配樂是電影動畫中的靈魂，不可或缺的技能！
                    </div>
                  </div>
                  <div class="mid-title__right">
                    <span>必學課程</span>
                    <span>48HRS</span>
                  </div>
                </div>
                <div class="mid-item">
                  <ul>
                    <li>軟硬體認識</li>
                    <li>音符與節奏</li>
                    <li>和弦記憶法</li>
                    <li>配器編曲</li>
                    <li>管弦樂設計</li>
                    <li>業界秘辛</li>
                    <li>成果交流</li>
                    <li>創作實務</li>
                    <li>作曲風格</li>
                    <li>基礎樂理</li>
                  </ul>
                  <div class="mid-music">
                    <div class="mid-music-title">
                      <div class="mid-music-title__left">
                        <img
                          src="@/assets/images/pic/pic_03_career.svg"
                          alt="圖片"
                        />
                      </div>
                      <p>舞台劇配樂 / 電視配樂 / 動畫配樂</p>
                    </div>
                    <div class="music-wrap">
                      <div class="music">
                        <div class="music-img">
                          <img
                            src="@/assets/images/pic/pic_03_music01_1x.jpeg"
                            alt="圖片"
                          />
                        </div>
                        <audio controls>
                          <source
                            src="@/assets/images/music/課程講師作品/08_電影動畫配樂創作/01.mp3"
                            type="audio/mpeg"
                          />
                        </audio>
                        <div class="music-info">
                          <img
                            src="@/assets/images/pic/pic_03_text8-1.svg"
                            alt="圖片"
                          />
                        </div>
                      </div>
                      <div class="music">
                        <div class="music-img">
                          <img
                            src="@/assets/images/pic/pic_03_music01_1x.jpeg"
                            alt="圖片"
                          />
                        </div>
                        <audio controls>
                          <source
                            src="@/assets/images/music/課程講師作品/08_電影動畫配樂創作/02.mp3"
                            type="audio/mpeg"
                          />
                        </audio>
                        <div class="music-info">
                          <img
                            src="@/assets/images/pic/pic_03_text8-2.svg"
                            alt="圖片"
                          />
                        </div>
                      </div>
                      <div class="music">
                        <div class="music-img">
                          <img
                            src="@/assets/images/pic/pic_03_music01_1x.jpeg"
                            alt="圖片"
                          />
                        </div>
                        <audio controls>
                          <source
                            src="@/assets/images/music/課程講師作品/08_電影動畫配樂創作/03.mp3"
                            type="audio/mpeg"
                          />
                        </audio>
                        <div class="music-info">
                          <img
                            src="@/assets/images/pic/pic_03_text8-3.svg"
                            alt="圖片"
                          />
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
              <div class="course-btn">
                <a class="cd-popup-trigger8" href="javascript:;"
                  >觀看完整課綱</a
                >
              </div>
            </div>
          </div>
          <CdPopup />
        </div>
      </div>
      <div class="s2-1-content-card">
        <div class="s2-1-content-title music-title-pc">
          <img src="@/assets/images/pic/pic_04_title.svg" alt="圖片" />
        </div>
        <div class="s2-1-content-title music-title-mb">
          <img src="@/assets/images/pic/mobile/pic_04_title04.svg" alt="圖片" />
        </div>
        <div class="s2-1-content-card-wrap">
          <div class="s2-1-content-left">
            <div class="s2-1-content-left-title-pc">
              <img src="@/assets/images/pic/pic_04-1.svg" alt="圖片" />
            </div>
            <div class="s2-1-content-left-title-mb">
              <img
                src="@/assets/images/pic/mobile/pic_04_title.svg"
                alt="圖片"
              />
            </div>
            <p>
              詞曲創作費用是預付版稅，預付可能$60K~$100K，依知名度調整費用。出版商協助詞曲創作者「機會媒合」、「著作授權」以及「收取授權費」，將透過簽定授權合約分潤收益，分潤比例普遍為出版商50%、詞曲創作人為50%，若議價能力、實力、談判技術好，詞曲創作人可談到75%，但得請創作人尋找專業律師協助。音樂出版商透過詞曲作者的「音樂著作」所被保障的權利如「公開演出權」、「同步錄音權」、「錄製權」，而這些權利透過商業行為轉換成版稅收益。
            </p>
          </div>
          <div class="s2-1-content-right">
            <div class="s2-1-content-right-img">
              <img src="@/assets/images/pic/pic_04-2.svg" alt="圖片" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import CdPopup from "@/components/CdPopup.vue";

export default {
  components: {
    CdPopup,
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

.course-area {
  position: relative;
}

.s2-title {
  width: 212.24px;
  height: 53.2px;
  margin: 0 auto;
  position: absolute;
  top: 0;
  left: 50%;
  margin-left: -106px;
  z-index: 1;

  @include min-width(768px) {
    width: 212.24px;
    height: 53.2px;
    margin-left: -106px;
  }

  @include min-width(1025px) {
    margin-top: -5rem;
  }

  @include min-width(1440px) {
    width: 265.3px;
    height: 66.5px;
    margin-left: -132.65px;
    margin-top: -5rem;
  }

  @include min-width(1920px) {
    width: 379px;
    height: 95px;
    margin-left: -189.5px;
    margin-top: -6rem;
  }

  .h2 {
    width: 100%;
    height: 100%;
    display: block;
    position: absolute;
    top: 0px;
    left: 0px;
    background: url("@/assets/images/pic/pic_03_COURSE.svg") no-repeat
      center/contain;
    @include hidetext;
  }
}
.s2-content {
  position: relative;
  border-bottom: 1px dashed $color-primary-1;
  border-left: 1px dashed $color-primary-1;
  border-bottom-left-radius: 50px;
  padding-top: 6rem;
  padding-bottom: 2rem;

  @include min-width(768px) {
    padding-top: 8rem;
    padding-bottom: 5rem;
  }

  @include min-width(1025px) {
    padding-top: 3rem;
  }
}
.s1-content-title {
  position: absolute;
  top: 0;
  margin-top: -7%;
  width: 100%;
  padding-bottom: 12.85%;
  background: url("@/assets/images/pic/pic_01_title.svg") no-repeat;
  background-size: contain;
  background-position: 0 100%;
}

.s2-content-cards {
  padding-left: 20px;
  width: 100%;

  @include min-width(1440px) {
    display: flex;
    justify-content: space-between;
    padding-left: 100px;
    padding-right: 50px;
  }

  .card-left {
    width: 100%;
    border: 1px solid $color-primary-1;

    &.card-list {
      .card-tags {
        display: none;

        @include min-width(1025px) {
          position: absolute;
          display: flex;
          align-items: center;
          top: 0px;
          left: 20px;
        }

        @include min-width(1440px) {
          display: block;
          top: 70px;
          left: 30px;
        }

        .level {
          padding: 0.5rem;
          background-color: $color-black;
          border: 1px solid $color-primary-1;
          color: $color-primary-1;
          font-weight: 700;
          font-size: 13px;

          @include min-width(1025px) {
            font-size: 20px;
          }

          &.level1 {
            margin-right: 1.2rem;

            @include min-width(1440px) {
              margin-bottom: 4rem;
              margin-right: 0;
            }
          }

          &.level2 {
            margin-right: 21rem;

            @include min-width(1440px) {
              margin-bottom: 22rem;
              margin-right: 0;
            }
          }

          @include min-width(1025px) {
            font-size: 16px;
            color: $color-white;
          }

          @include min-width(1440px) {
            font-size: 20px;
            color: $color-primary-1;
          }
        }
      }

      .card-list-nav {
        width: 100%;
        display: flex;
        //justify-content: space-between;
        flex-wrap: nowrap;
        //white-space: nowrap;
        overflow-x: auto;

        @include min-width(1440px) {
          width: auto;
          display: block;
        }

        > a {
          //width: 13%;
          //margin: 0 12px;
          flex: none;
          padding: 8px 13.7px;
          position: relative;
          display: block;
          cursor: pointer;
          transition: all 0.2s ease;
          border-right: 1px solid $color-primary-1;

          &:first-child {
            margin-top: 0;
          }

          &:last-child {
            border-right: none;
          }

          @include min-width(1280px) {
          }

          @include min-width(1440px) {
            margin-right: 0;
            margin-left: auto;
            padding: 0;
            margin-top: 1rem;
            width: 65%;
            border-right: none;

            &:before,
            &:after {
              content: "";
              position: absolute;
              top: 0;
              left: -50px;
              display: block;
            }

            &:before {
              width: 14px;
              height: 14px;
              border-radius: 50%;
              border: 2px solid $color-primary-1;
              background-color: $color-black;
              z-index: 5;
            }

            &:after {
              left: -42px;
              width: 1px;
              height: 100px;
              background-color: $color-primary-1;
            }

            &:last-child {
              &:after {
                display: none;
              }
            }
          }

          > span {
            display: block;
            font-weight: 400;
            font-size: 14px;
            text-align: center;
            color: $color-white;

            &:first-child {
              font-weight: 700;
              font-size: 14px;
              color: $color-primary-1;

              @include min-width(1440px) {
                font-size: 18px;
              }
            }

            &:last-child {
              display: none;

              @include min-width(1440px) {
                display: block;
              }
            }

            @include min-width(1440px) {
              text-align: left;
            }
          }

          &.active {
            background-color: $color-primary-1;

            > span {
              color: $color-white;
            }

            @include min-width(1440px) {
              background-color: transparent;

              &:before {
                content: "";
                border: 2px solid $color-white;
                background-color: $color-primary-1;
              }
            }
          }
        }
      }
    }

    @include min-width(1025px) {
      display: flex;
    }

    @include min-width(1440px) {
      width: 30%;
      padding: 35px;
      border-radius: 16px;
      display: block;
      background: linear-gradient(
        137.1deg,
        rgba(0, 224, 184, 0.1) 14.56%,
        rgba(0, 224, 184, 0.1) 85.34%
      );
    }
  }

  .card-right {
    width: 100%;
    margin-top: 3rem;
    padding: 20px;
    border: 1px solid $color-primary-1;
    position: relative;

    @include min-width(1025px) {
      margin-top: 0;
      padding-bottom: 100px;
      border-top: none;
      padding: 45px 100px;
    }

    @include min-width(1440px) {
      width: 68.5%;
      padding: 45px;
      border: 1px solid $color-primary-1;
      border-radius: 16px;
    }

    .card-lines {
      @include min-width(1440px) {
        margin-top: -300px;
        height: 600px;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        position: absolute;
        top: 50%;
        left: -35px;

        > span {
          width: 45px;
          height: 16px;
          display: block;
          border-radius: 32px;
          border: 1px solid $color-primary-1;
          background-color: $color-black;
        }
      }
    }
  }
}

.card-pages {
  .mid {
    .mid-title {
      @include min-width(1025px) {
        display: flex;
        justify-content: space-between;
        align-items: flex-end;
      }

      .mid-title__left {
        width: 100%;

        @include min-width(1025px) {
          width: 66%;
        }

        @include min-width(1440px) {
          width: 68%;
        }

        @include min-width(1920px) {
          width: 66%;
        }

        .mid-title__left-t {
          display: flex;
          align-items: center;

          .mid-title__left-img {
            width: 55%;
            margin-right: 1rem;

            @include min-width(768px) {
              width: auto;
            }

            @include min-width(1440px) {
              width: 60%;
            }

            > img {
              width: 100%;
            }
          }

          > span {
            display: block;
            color: $color-primary-1;
            font-weight: 700;
            font-size: 18px;

            @include min-width(768px) {
              font-size: 20px;
            }

            @include min-width(1025px) {
              font-size: 18px;
            }
          }
        }

        .mid-title__left-b {
          margin-top: 1rem;
          font-weight: 400;
          font-size: 13px;
          color: $color-white;

          @include min-width(768px) {
            font-size: 20px;
          }
        }
      }

      .mid-title__right {
        width: 100%;
        margin-top: 2rem;
        display: flex;
        justify-content: flex-start;
        align-items: flex-end;

        @include min-width(1025px) {
          width: 30%;
          margin-top: 0;
          justify-content: flex-end;
        }

        > span {
          display: block;
          font-weight: 400;
          font-size: 16px;
          color: $color-primary-1;

          &:nth-child(1) {
            margin-right: 0.5rem;
          }
          &:nth-child(2) {
            font-weight: 800;
            font-size: 24px;
            color: $color-primary-7;

            @include min-width(768px) {
              font-size: 30px;
            }
          }
        }
      }
    }

    .mid-item {
      margin-top: 3rem;

      > ul {
        width: 100%;
        display: flex;
        justify-content: flex-start;
        flex-wrap: wrap;
        padding-bottom: 2rem;
        border-bottom: 1px dashed $color-primary-1;

        @include min-width(1025px) {
          padding-bottom: 0;
          justify-content: space-between;
        }

        > li {
          width: 28%;
          display: flex;
          justify-content: center;
          align-items: center;
          position: relative;
          margin-right: 1rem;
          margin-bottom: 3rem;
          padding: 0.5rem 0;
          border: 1px solid $color-primary-1;
          border-radius: 10px;
          text-align: center;
          color: $color-white;
          font-size: 16px;

          &:nth-child(5n + 5) {
            margin-right: 0;
          }

          &:nth-child(1),
          &:nth-child(2),
          &:nth-child(3),
          &:nth-child(4) {
            &:after {
              content: "";
              width: 16px;
              height: 24px;
              display: block;
              position: absolute;
              right: -30px;
              background: url("@/assets/images/pic/pic_03_arrow.svg") no-repeat
                center/contain;
            }
          }
          &:nth-child(5) {
            &:after {
              content: "";
              width: 16px;
              height: 24px;
              display: block;
              position: absolute;
              top: 45px;
              transform: rotate(90deg);
              background: url("@/assets/images/pic/pic_03_arrow.svg") no-repeat
                center/contain;
            }
          }

          &:nth-child(6),
          &:nth-child(7),
          &:nth-child(8),
          &:nth-child(9) {
            &:after {
              content: "";
              width: 16px;
              height: 24px;
              display: block;
              position: absolute;
              transform: scaleX(-1);
              right: -30px;
              background: url("@/assets/images/pic/pic_03_arrow.svg") no-repeat
                center/contain;
            }
          }

          @include max-width(1025px) {
            width: 26.5%;
            margin-right: 3rem;
            margin-bottom: 1rem;

            &:nth-child(3n + 3) {
              margin-right: 0;
            }

            &:nth-child(5n + 5) {
              margin-right: 3rem;
            }

            &:nth-child(1),
            &:nth-child(2),
            &:nth-child(3),
            &:nth-child(4) {
              &:after {
                content: "";
                width: 16px;
                height: 24px;
                display: block;
                position: absolute;
                right: -35px;
                background: url("@/assets/images/pic/pic_03_arrow.svg")
                  no-repeat center/contain;
              }
            }

            &:nth-child(5) {
              &:after {
                content: "";
                width: 16px;
                height: 24px;
                top: auto;
                right: -35px;
                transform: rotate(360deg);
                display: block;
                background: url("@/assets/images/pic/pic_03_arrow.svg")
                  no-repeat center/contain;
              }
            }

            &:nth-child(6),
            &:nth-child(7),
            &:nth-child(8),
            &:nth-child(9) {
              &:after {
                content: "";
                width: 16px;
                height: 24px;
                display: block;
                position: absolute;
                transform: scaleX(1);
                right: -35px;
                background: url("@/assets/images/pic/pic_03_arrow.svg")
                  no-repeat center/contain;
              }
            }
          }

          @include min-width(1025px) {
            width: 15%;
          }

          @include max-width(768px) {
            margin-bottom: 1rem;
            margin-right: 2.5rem;
            font-size: 14px;

            &:nth-child(3n + 3) {
              margin-right: 0;
            }

            &:nth-child(5n + 5) {
              margin-right: 2.5rem;
            }

            &:nth-child(1),
            &:nth-child(2),
            &:nth-child(3),
            &:nth-child(4) {
              &:after {
                content: "";
                width: 16px;
                height: 24px;
                display: block;
                position: absolute;
                right: -25px;
                background: url("@/assets/images/pic/pic_03_arrow.svg")
                  no-repeat center/contain;
              }
            }

            &:nth-child(5) {
              &:after {
                content: "";
                width: 16px;
                height: 24px;
                top: auto;
                right: -25px;
                transform: rotate(360deg);
                display: block;
                background: url("@/assets/images/pic/pic_03_arrow.svg")
                  no-repeat center/contain;
              }
            }

            &:nth-child(6),
            &:nth-child(7),
            &:nth-child(8),
            &:nth-child(9) {
              &:after {
                content: "";
                width: 16px;
                height: 24px;
                display: block;
                position: absolute;
                transform: scaleX(1);
                right: -25px;
                background: url("@/assets/images/pic/pic_03_arrow.svg")
                  no-repeat center/contain;
              }
            }
          }

          @include max-width(484px) {
            margin-bottom: 1rem;
            margin-right: 1.5rem;

            &:nth-child(3n + 3) {
              margin-right: 0;
            }

            &:nth-child(5n + 5) {
              margin-right: 1.5rem;
            }

            &:nth-child(1),
            &:nth-child(2),
            &:nth-child(3),
            &:nth-child(4) {
              &:after {
                content: "";
                width: 13px;
                height: 24px;
                display: block;
                position: absolute;
                right: -20px;
                background: url("@/assets/images/pic/pic_03_arrow.svg")
                  no-repeat center/contain;
              }
            }

            &:nth-child(5) {
              &:after {
                content: "";
                width: 13px;
                height: 24px;
                top: auto;
                right: -20px;
                transform: rotate(360deg);
                display: block;
                background: url("@/assets/images/pic/pic_03_arrow.svg")
                  no-repeat center/contain;
              }
            }

            &:nth-child(6),
            &:nth-child(7),
            &:nth-child(8),
            &:nth-child(9) {
              &:after {
                content: "";
                width: 13px;
                height: 24px;
                display: block;
                position: absolute;
                transform: scaleX(1);
                right: -20px;
                background: url("@/assets/images/pic/pic_03_arrow.svg")
                  no-repeat center/contain;
              }
            }
          }
        }
      }

      .mid-music {
        margin-top: 2rem;

        .mid-music-title {
          @include min-width(1025px) {
            display: flex;
            align-items: center;
          }

          > p {
            margin-top: 1rem;
            margin-bottom: 0;
            font-size: 16px;
            color: $color-primary-1;

            @include min-width(1025px) {
              margin-top: 0;
              margin-left: 0.5rem;
            }
          }
        }

        .mid-music-title__left {
          width: 50%;

          @include min-width(768px) {
            width: 30%;
          }

          @include min-width(1025px) {
            width: auto;
          }

          > img {
            width: 100%;
          }
        }

        .music-wrap {
          margin-top: 1.5rem;

          @include min-width(768px) {
            padding: 0 5rem;
          }

          @include min-width(1025px) {
            padding: 0;
            display: flex;
            justify-content: space-between;
          }

          .music-wrap-left {
            width: 100%;

            @include min-width(1025px) {
              width: 68%;
            }

            > video {
              width: 100%;
            }
          }

          .music-wrap-right {
            width: 100%;
            display: flex;
            align-items: center;
            justify-content: center;

            @include min-width(1025px) {
              width: 28%;
            }

            .music-wrap-right-img {
              width: 100%;
              display: flex;
							margin-top: 2rem;
							margin-bottom: 5rem;

              @include min-width(1025px) {
                width: auto;
								margin-top: 0;
								margin-bottom: 0;
              }

              > img {
                width: 100%;
                margin: 0 auto;
              }
            }
          }
        }

        .music {
          width: 100%;
          margin-bottom: 2rem;
					

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
            margin-top: 1rem;
            width: 100%;

            @include min-width(1025px) {
              margin-top: 0.75rem;
              height: 30px;
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
  }

  .course-btn {
    position: absolute;
    bottom: -35px;
    left: 50%;
    margin-left: -143.04px;

    @include min-width(768px) {
      bottom: -50px;
      margin-left: -178.8px;
    }

    @include min-width(1440px) {
      margin-left: -223.5px;
    }

    > a {
      display: block;
      width: 286.08px;
      height: 69.76px;
      background: url("@/assets/images/btn/btn_syllabus_default.svg") no-repeat
        center/contain;
      @include hidetext;
      transition: 0.2s;

      @include min-width(768px) {
        width: 357.6px;
        height: 87.2px;
      }

      @include min-width(1025px) {
        &:hover {
          background: url("@/assets/images/btn/btn_syllabus_hover.svg")
            no-repeat center/contain;
        }
      }

      @include min-width(1440px) {
        width: 447px;
        height: 109px;
      }
    }
  }
}

.s2-1-content-card {
  margin-top: 5rem;
  padding-left: 20px;
  padding-right: 20px;

  @include min-width(768px) {
    padding-left: 50px;
    padding-right: 50px;
  }

  @include min-width(1440px) {
    padding-left: 100px;
  }

  .s2-1-content-title {
    width: 100%;

    @include min-width(1025px) {
      width: 60%;
    }

    > img {
      width: 100%;
    }
  }

  .s2-1-content-card-wrap {
    margin-top: 2rem;

    @include min-width(1025px) {
      display: flex;
      justify-content: space-between;
    }

    .s2-1-content-left {
      width: 100%;

      @include min-width(1025px) {
        width: 35%;
        padding-left: 80px;
      }

      @include min-width(1280px) {
        padding-left: 20px;
      }

      @include min-width(1440px) {
        width: 38%;
        height: auto;
        padding-left: 40px;
      }

      @include min-width(1920px) {
        width: 35%;
        padding-left: 80px;
      }

      > p {
        margin-top: 2rem;
        margin-bottom: 3rem;
        text-align: justify;
        color: $color-white;
        font-size: 16px;
        line-height: 32px;
        overflow-y: auto;

        @include min-width(1025px) {
          margin-bottom: 1rem;
          height: 250px;
          font-size: 13px;
        }

        @include min-width(1280px) {
          height: auto;
        }

        @include min-width(1440px) {
          font-size: 16px;
          line-height: 30px;
        }
      }
    }

    .s2-1-content-left-title-pc {
      display: none;

      @include min-width(1025px) {
        display: block;
      }
    }

    .s2-1-content-left-title-mb {
      width: 100%;
      display: block;
      margin: 0 auto;

      > img {
        width: 100%;
      }

      @include min-width(768px) {
        width: 50%;
      }

      @include min-width(1025px) {
        display: none;
      }
    }

    .s2-1-content-right {
      width: 100%;

      @include min-width(1025px) {
        width: 60%;
      }

      @include min-width(1440px) {
        width: 55%;
      }

      @include min-width(1920px) {
        width: 60%;
      }

      .s2-1-content-right-img {
        > img {
          width: 100%;
        }
      }
    }
  }

  .music-title-pc {
    display: none;

    @include min-width(1025px) {
      display: block;
    }
  }

  .music-title-mb {
    width: 100%;
    margin: 0 auto;
    display: block;

    @include min-width(768px) {
      width: 50%;
    }

    @include min-width(1025px) {
      display: none;
    }
  }
}
</style>