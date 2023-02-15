<template>
  <div class="cd-popup" role="alert">
    <div class="cd-popup-container">
      <div class="cd-popup-container-left">
        <div class="s4-content-title"></div>
        <div class="swiper-bg"></div>
        <div class="cd-popup-container-left-bottom">
          <div class="swiper popup-swiper-form">
            <div class="swiper-tag">
              <img src="@/assets/images/pic/pic_07_subtitle.svg" alt="圖片" />
            </div>
            <div class="swiper-wrapper">
              <div class="swiper-slide">
                <div class="main-banner">
                  <img src="@/assets/images/pic/pic_07-1_p1.svg" alt="圖片" />
                </div>
              </div>
              <div class="swiper-slide">
                <div class="main-banner">
                  <img src="@/assets/images/pic/pic_07-1_p2.svg" alt="圖片" />
                </div>
              </div>
              <div class="swiper-slide">
                <div class="main-banner">
                  <img src="@/assets/images/pic/pic_07-1_p3.svg" alt="圖片" />
                </div>
              </div>
            </div>
            <div class="swiper-border swiper-border-l"></div>
            <div class="swiper-border swiper-border-r"></div>
            <div class="swiper-pagination"></div>
            <div class="swiper-button-next next"></div>
            <div class="swiper-button-prev prev"></div>
          </div>
        </div>
      </div>
      <!--表單-->
      <div id="4" class="cd-popup-container-right">
        <div class="cd-popup-container-right-top">
          <div class="top-img">
            <img src="@/assets/images/pic/pic_07-3_title.svg" alt="圖片" />
          </div>
          <span>每日限量20名免費索取</span>
        </div>
        <div class="cd-popup-container-right-bottom">
          <div class="popup-form _form">
            <form id="contact-form" class="form-distribution">
              <!--設定表單參數-->
              <input name="distribution" type="text" hidden value="4" />
              <!--副類別-->
              <input name="outletSub" type="text" hidden value="213" />
              <!--媒體版位-->
              <input name="mediaSub" type="text" hidden value="823" />
              <input name="type" type="text" hidden value="Event" />
              <input name="course" type="text" hidden value="音樂製作課程" />
              <input name="gift" type="text" hidden value="線上課程+實體講堂" />
              <!--設定表單參數-->
              <div class="fieldset">
                <!--姓名-->
                <fieldset>
                  <input
                    class="fieldset-input"
                    placeholder="真實姓名*"
                    type="text"
                    name="name"
                    tabindex="1"
                  />
                </fieldset>

                <!--手機-->
                <fieldset>
                  <input
                    class="fieldset-input"
                    placeholder="手機號碼*"
                    type="tel"
                    name="cellphone"
                    tabindex="2"
                  />
                </fieldset>

                <!--城市-->
                <fieldset>
                  <div class="select-form">
                    <select
                      id="city"
                      class="select-form-block"
                      name="city"
                      tabindex="3"
                    >
                      <option value="">請選縣市</option>
                    </select>

                    <select
                      id="area"
                      class="select-form-block"
                      name="area"
                      tabindex="4"
                    >
                      <option value="">請選地區</option>
                    </select>
                  </div>
                </fieldset>

                <!--信箱-->
                <fieldset>
                  <input
                    class="fieldset-input"
                    placeholder="電子信箱*"
                    type="email"
                    name="email"
                    tabindex="5"
                  />
                </fieldset>

                <!--參加地區-->
                <fieldset>
                  <legend class="fieldset-title">
                    你對音樂製作的瞭解程度？
                  </legend>
                  <label class="input-check">
                    <input
                      class="checkbox styled-checkbox"
                      type="radio"
                      name="zip"
                      value="value1"
                      data-value="零基礎"
                      data-mail_id="25"
                      tabindex="6"
                    />
                    <span>零基礎</span>
                  </label>
                  <label class="input-check">
                    <input
                      class="checkbox styled-checkbox"
                      type="radio"
                      name="zip"
                      value="value2"
                      data-value="初學者"
                      data-mail_id="26"
                      tabindex="7"
                    />
                    <span>初學者</span>
                  </label>
                  <label class="input-check">
                    <input
                      class="checkbox styled-checkbox"
                      type="radio"
                      name="zip"
                      value="value3"
                      data-value="專業職人"
                      data-mail_id="27"
                      tabindex="8"
                    />
                    <span>專業職人</span>
                  </label>
                </fieldset>

                <!--詢問相關問題-->
                <fieldset>
                  <textarea
                    id="message_area"
                    class="fieldset-input"
                    placeholder="想詢問音樂製作相關問題..."
                    name="message_area"
                    tabindex="10"
                  ></textarea>
                </fieldset>

                <!--詳細閱讀-->
                <fieldset class="field">
                  <label class="input-checkbox flex justify-center align-items">
                    <input
                      type="checkbox"
                      name="agreement"
                      value="horror"
                    /><span class="privacy-check"></span>
                    <span class="privacy-text"
                      >我已詳細閱讀並同意<a
                        href="https://www.appedu.com.tw/frame-privacy"
                        target="_blank"
                        class="form-privacy"
                        >隱私權使用條款</a
                      >
                    </span>
                  </label>
                  <span class="from-txt"
                    >填寫完表單後，請點擊【立即領取】可立即領取好禮，
                    填寫成功訊息將回傳至您填寫的Email信箱以及手機簡訊。</span
                  >
                </fieldset>

                <!--送出按鈕-->
                <div class="btn-submit-wrap">
                  <input
                    class="btn-submit"
                    type="submit"
                    name="submit"
                    value="填寫完成"
                  />
                </div>
              </div>
            </form>
          </div>
        </div>
      </div>
    </div>
    <!-- cd-popup-container -->
  </div>
</template>

<script>
export default {
  mounted() {
    $(document).ready(function () {
      var GET_LOCATION_ENDPOINT =
        "https://www.appedu.com.tw/Librarys/_ajax/Address.php";
      var DISTRIBUTION_ENDPOINT =
        "https://www.appedu.com.tw/Librarys/_ajax/Distribution.php";

      function loadLocation(options) {
        var $cityElement = options.city.element;
        var $areaElement = options.area.element;
        $cityElement.html(
          $("<option>").text(options.city.defaultLabel).val("")
        );
        $areaElement.html(
          $("<option>").text(options.area.defaultLabel).val("")
        );
        // load city data
        $.ajax({
          url: GET_LOCATION_ENDPOINT,
          type: "POST",
          dataType: "json",
          data: { postFlag: "LoadCity" },
        })
          .done(function (response) {
            if (response.result == "true") {
              response.data.forEach(function (v) {
                $cityElement.append($("<option>").val(v.id).text(v.name));
              });
            }
          })
          .fail(function () {
            alert(options.city.errorMessage);
          });
        // listen to city and load area data
        $cityElement.change(function () {
          $areaElement.html(
            $("<option>").text(options.area.defaultLabel).val("")
          );
          $.ajax({
            url: GET_LOCATION_ENDPOINT,
            type: "POST",
            dataType: "json",
            data: {
              postFlag: "LoadArea",
              CityID: $(this).val(),
            },
          })
            .done(function (response) {
              if (response.result == "true") {
                response.data.forEach(function (v) {
                  $areaElement.append($("<option>").val(v.id).text(v.name));
                });
              }
            })
            .fail(function () {
              alert(options.area.errorMessage);
            });
        });
      }

      $.validator.addMethod(
        "cellphone",
        function (value, element) {
          var reg = /^[09]{2}[0-9]{8}$/;
          return this.optional(element) || reg.test(value);
        },
        "Please enter a valid cellphone."
      );

      /*
參數兼容4種設定方式
distributionSubmitHandler("成功");
distributionSubmitHandler({ success: "成功", error: "失敗" });
distributionSubmitHandler({
  success: function(response) {
    alert("成功");
  },
  error: function(response) {
    alert("失敗");
  }
});
distributionSubmitHandler(function(response){
  if (response.result == "true") {
    alert("成功");
  } else {
    alert("失敗");
  }
});
*/
      function distributionSubmitHandler(options) {
        return function (form) {
          let $checkbox = $(".styled-checkbox:checked");
          let $message_area = $("#message_area");
          let remark_text =
            "我是：" +
            $checkbox.data("value") +
            "，" +
            "我想詢問：" +
            $message_area.val();
          $.ajax({
            url: DISTRIBUTION_ENDPOINT,
            type: "POST",
            dataType: "json",
            data: {
              postFlag: "InsertData",
              distribution_id: form.distribution.value,
              media_sub_id: form.mediaSub.value,
              outlet_sub_id: form.outletSub.value,
              type: form.type.value,
              course: form.course.value,
              name: form.name.value,
              cellphone: form.cellphone.value,
              email: form.email.value,
              zip_id: form.area.value,
              remark: remark_text,
              gift: form.gift && form.gift.value,
              sms_id: 29,
              mail_id: $checkbox.data("mail_id"),
            },
          })
            .done(function (response) {
              if (typeof options == "function") {
                return options(response);
              }
              var opt = { success: null, error: null };
              if ($.isPlainObject(options)) {
                $.extend(opt, options);
              } else {
                opt.success = options;
              }
              // 舊版本相容
              if (!options.success && options.successMessage) {
                options.success = options.successMessage;
                // 舊版 errorMessage 根本沒用到，不覆蓋以維持舊頁面原樣
              }
              if (response.result == "true") {
                if (typeof options.success == "function") {
                  return options.success(response);
                } else {
                  alert(options.success);
                  top.location.href =
                    "https://www.appedu.com.tw/Event/musicproduction-series/";
                }
              } else {
                if (typeof options.error == "function") {
                  return options.error(response);
                } else {
                  alert("資料送出失敗，請聯絡我們或再試一次");
                }
              }
            })
            .fail(function (error) {
              console.error(error);
              alert("網路問題無法傳送資料，請聯絡我們或再試一次");
            });
          return false;
        };
      }

      var $form = $("form.form-distribution");
      loadLocation({
        city: {
          element: $form.find("[name=city]"),
          defaultLabel: "請選縣市",
          errorMessage: "無法載入縣市資料",
        },
        area: {
          element: $form.find("[name=area]"),
          defaultLabel: "請選地區",
          errorMessage: "無法載入地區資料",
        },
      });

      $form
        .submit(function (e) {
          e.preventDefault();
        })
        .validate({
          // debug: true,
          submitHandler: distributionSubmitHandler({
            successMessage: "資料已送出，將安排專人與您聯絡",
            errorMessage: "您輸入的資料有誤或者已輸入過相同資料",
          }),
          rules: {
            name: "required",
            email: { required: true, email: true },
            cellphone: { required: true, cellphone: true },
            city: "required",
            area: "required",
            remark: "required",
            course: "required",
            agreement: "required",
          },
          messages: {
            name: "請輸入您的姓名",
            email: {
              required: "請輸入您的E-mail信箱",
              email: "請輸入有效的E-mail信箱",
            },
            cellphone: {
              required: "請輸入您的聯絡電話",
              cellphone: "請輸入有效的聯絡電話",
            },
            city: "請選擇居住縣市與地區",
            area: "請選擇居住縣市與地區",
            remark: "",
            course: "請選擇想學課程",
            agreement: "您尚未接受隱私權使用條款",
          },
        });
    });

    var swiper3 = new Swiper(".popup-swiper-form", {
      pagination: {
        el: ".popup-swiper-form .swiper-pagination",
        clickable: true,
      },
      navigation: {
        nextEl: ".next",
        prevEl: ".prev",
      },
    });
  },
};
</script>

<style lang="scss">
@import "@/assets/scss/mixin.scss";
@import "@/assets/scss/variables.scss";
@import "@/assets/scss/from-option.scss";
@import "@/assets/scss/from.scss";

.cd-popup-container-left {
  position: relative;
  margin-top: 20rem;

  @include min-width(768px) {
    margin-top: 25rem;
  }

  @include min-width(1025px) {
    width: 55%;
    margin-top: 0;
    margin-right: -6px;
  }

  @include min-width(1440px) {
    width: 50%;
    margin-right: -6px;
    margin-left: auto;
  }

  .s4-content-title {
    margin-top: -33%;
    margin-left: 3%;
    width: 100%;
    padding-bottom: 29.32%;
    z-index: 10;
    background: url("@/assets/images/pic/mobile/pic_07_title07.svg") no-repeat;
    background-size: contain;
    background-position: 0 100%;

    @include min-width(768px) {
      width: 50%;
      margin-top: -22%;
      margin-left: 25%;
      padding-bottom: 17.34%;
    }

    @include min-width(1025px) {
      position: absolute;
      top: 0;
      width: 100%;
      margin-top: 5%;
      margin-left: -3rem;
      padding-bottom: 25.34%;
      background: url("@/assets/images/pic/pic_07_title.svg") no-repeat;
      background-size: contain;
      background-position: 0 100%;
    }

    @include min-width(1280px) {
      margin-top: 22%;
    }

    @include min-width(1440px) {
      margin-top: 7%;
    }

    @include min-width(1920px) {
      margin-top: 5%;
    }
  }
}

//RIGHT

.cd-popup-container-right-top {
  position: relative;

  .top-img {
    width: 50%;
    margin: 0 auto;
    margin-top: 2rem;

    > img {
      width: 100%;
    }
  }

  > span {
    display: block;
    margin-top: 1rem;
    text-align: center;
    font-size: 18px;
    color: $color-white;
  }

  &::after {
    content: "";
    width: 91px;
    height: 146px;
    position: absolute;
    top: -100px;
    right: 0;
    display: block;
    background: url("@/assets/images/pic/pic_07-2_note.svg") no-repeat
      center/contain;
  }
}

.cd-popup-container-right {
  width: 100%;
  margin-right: 0;
  position: relative;
  z-index: 10;
  //margin: 0 auto;
  padding: 0.3rem;
  border: 1px solid transparent;
  border-radius: 25px;
  background-image: linear-gradient($color-black, $color-black),
    linear-gradient(to right, #fff176, #00e0b8);
  background-origin: border-box;
  background-clip: content-box, border-box;

  @include min-width(1025px) {
    width: 45%;
  }

  @include min-width(1440px) {
    width: 40%;
  }
}

.cd-popup-container-right-top-title {
  font-weight: 400;
  font-size: 22px;
  line-height: 33px;
  color: $color-black;
  text-align: center;

  @include min-width(1025px) {
    font-size: 26px;
  }
}

.cd-popup-container-right-top-subtitle {
  font-weight: 400;
  font-size: 14px;
  line-height: 22px;
  color: $color-black;
  text-align: center;

  @include min-width(1025px) {
    font-size: 18px;
  }
}

.swiper-bg {
  @include min-width(1025px) {
    position: absolute;
    top: 50%;
    margin-top: -280px;
    width: 100%;
    padding-bottom: 83.11%;
    background: url("@/assets/images/pic/pic_07-4_bg.png") no-repeat
      center/contain;
  }

  @include min-width(1280px) {
    margin-top: -233.75px;
    padding-bottom: 100%;
  }

  @include min-width(1440px) {
    margin-top: -270px;
    padding-bottom: 83.11%;
  }

  @include min-width(1920px) {
    margin-top: -280px;
  }
}

.cd-popup-container-left-bottom {
  position: relative;
  margin-top: 4rem;

  @include min-width(1025px) {
    margin-top: 5rem;
    padding: 4rem;
  }

  @include min-width(1280px) {
    margin-top: 10rem;
    padding: 4rem;
  }

  @include min-width(1440px) {
    margin-top: 7rem;
    padding: 8rem;
  }

  @include min-width(1920px) {
    margin-top: 10rem;
  }
}

.input-checkbox {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 0 5.5px;
  line-height: 25px;
  cursor: pointer;
}

.privacy-check {
  margin-right: 1rem;
  display: none !important;
}

.field {
  margin-top: 2rem !important;
}

.from-txt {
  margin-top: 2rem;
  display: block;
  font-size: 12px;
  line-height: 16.8px;
  color: $color-white;
	text-align: center;

	@include min-width(768px) {
		padding: 0 4rem;
		text-align: left;
	}

  @include min-width(1440px) {
    padding: 0 2rem;
  }

  @include min-width(1920px) {
    padding: 0 4rem;
  }
}

.swiper-tag {
  width: 35%;
  margin: 0 auto;

  > img {
    width: 100%;
  }

	@include min-width(768px) {
		width: 20%;
	}

  @include min-width(1025px) {
    position: absolute;
    top: 0;
    left: 50%;
    width: 25%;
    margin-top: 4.5rem;
    margin-left: -64.28px;
  }

  @include min-width(1440px) {
    width: auto;
    margin-top: 4rem;
    margin-left: -80px;
  }
}

.swiper-border {
  position: absolute;
  top: 0%;
  width: 30px;
  height: calc(100% - 150px);

  @include min-width(1025px) {
    top: 50%;
    height: calc(100% - 150px);
    margin-top: -135px;
  }

  @include min-width(1440px) {
    height: calc(100% - 300px);
    margin-top: -155px;
  }

  &.swiper-border-l {
    left: 50px;
    border-top: 1px solid $color-primary-1;
    border-bottom: 1px solid $color-primary-1;
    border-left: 1px solid $color-primary-1;

    @include min-width(1025px) {
      left: 80px;
    }

    @include min-width(1440px) {
      left: 135px;
    }
  }

  &.swiper-border-r {
    right: 50px;
    border-top: 1px solid $color-primary-1;
    border-bottom: 1px solid $color-primary-1;
    border-right: 1px solid $color-primary-1;

    @include min-width(1025px) {
      right: 80px;
    }

    @include min-width(1440px) {
      right: 135px;
    }
  }
}

.next {
  @include min-width(1025px) {
    margin-top: -25px !important;
    right: 40px !important;
  }

  @include min-width(1440px) {
    margin-top: -50px !important;
    right: 100px !important;
  }
}

.prev {
  @include min-width(1025px) {
    margin-top: -25px !important;
    left: 40px !important;
  }

  @include min-width(1440px) {
    margin-top: -50px !important;
    left: 100px !important;
  }
}
</style>