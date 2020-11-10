<template>
  <div>
    <div class="banner-container">
      <div class="overlay">
        <img src="../assets/banner.png">

        <div class="banner-text">
          <div class="main-text">
            7 DAYS BETTER YOU
          </div>
          <div class="sub-text">
            เนื้อหาจำลองแบบเรียบๆ ที่ใช้กันในธุรกิจงานพิมพ์หรืองานเรียงพิมพ์ มันได้กลายมาเป็นเนื้อหาจำลองมาตรฐานของธุรกิจดังกล่าวมาตั้งแต่ศตวรรษที่ 16
          </div>
          <a-button class="custom-button" type="primary">
            สมัครสมาชิก
          </a-button>
        </div>

        <div class="banner-block-container">
          <div class="banner-block">
            <div class="banner-block-list">
              <div class="banner-block-list-text">
                <div class="banner-block-list-main-text">
                  โดยผู้เชี่ยวชาญ
                </div>
                <div class="banner-block-list-sub-text">
                  เนื้อหาจำลองแบบเรียบๆ ที่ใช้กันในธุรกิจงานพิมพ์
                </div>
              </div>
              <div class="banner-block-list-icon">
                <img src="../assets/ic-banner1.svg">
              </div>
            </div>
            <div class="banner-block-list">
              <div class="banner-block-list-text">
                <div class="banner-block-list-main-text">
                  ได้ผลจริง
                </div>
                <div class="banner-block-list-sub-text">
                  เนื้อหาจำลองแบบเรียบๆ ที่ใช้กันในธุรกิจงานพิมพ์
                </div>
              </div>
              <div class="banner-block-list-icon">
                <img src="../assets/ic-banner2.svg">
              </div>
            </div>            <div class="banner-block-list">
              <div class="banner-block-list-text">
                <div class="banner-block-list-main-text">
                  ทุกที่ทุกเวลา
                </div>
                <div class="banner-block-list-sub-text">
                  เนื้อหาจำลองแบบเรียบๆ ที่ใช้กันในธุรกิจงานพิมพ์
                </div>
              </div>
              <div class="banner-block-list-icon">
                <img src="../assets/ic-banner3.svg">
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="ads">
        <div class="ads-content">
          <div class="ads-main-text">
            เปลี่ยนเป็นคุณคนใหม่ใน 7 วัน
          </div>
          <div class="ads-sub-text">
            <p>เนื้อหาจำลองแบบเรียบๆ ที่ใช้กันในธุรกิจงานพิมพ์หรืองานเรียงพิมพ์</p>
            <p>มันได้กลายมาเป็นเนื้อหาจำลองมาตรฐานของธุรกิจดังกล่าวมาตั้งแต่ศตวรรษที่ 16</p>
          </div>
          <div class="ads-img">
              <img src='../assets/image1.png'>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  components: {
  }
}
</script>

<style lang="scss" scoped>
.banner-container {
    width: 100%;
    height: 560px;
    background-color: $based-color;

    & > .overlay {
        width: 100%;
        height: 560px;
        position: relative;

        & > img {
            width: 100%;
            height: 560px;
            object-fit: cover;
        }
        & > .banner-text {
            position: absolute;
            top:122px;
            color:#fff;
            width: 100%;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;

            & > .main-text {
                font-weight: 500;
                font-size:40px;
                text-align: center;
            }

            & > .sub-text {
                font-size: 0.875rem;
                text-align: center;
                width: 560px;
                font-weight: 400;
                margin:0 auto;
                opacity: 0.85;
                margin:20px 0 37px 0;
            }
        }

        & > .banner-block-container {
            width: 100%;
            height: 127px;
            display: flex;
            justify-content: center;
            position: absolute;
            bottom:0;

            & > .banner-block {
                position: absolute;
                width: 960px;
                height: 127px;
                background-color: rgb(255,255,255,0.3);
                bottom: 0;
                border-radius: 6px 6px 0px 0px;
                display: flex;

                & > .banner-block-list {
                    flex:1;
                    display: flex;
                    justify-content: space-between;
                    padding:32px;

                    &:first-child {
                        border-right:rgb(255,255,255,0.25) 1px solid ;
                    }
                    &:last-child {
                        border-left:rgb(255,255,255,0.25) 1px solid ;
                    }

                    & > .banner-block-list-text {
                        display: flex;
                        flex-direction: column;
                        color:#fff;

                        & > .banner-block-list-main-text {
                            font-size: 16px;
                            font-weight: 700;
                            margin-bottom: 5px;

                        }
                        & > .banner-block-list-sub-text {
                            font-size: 12px;
                            font-weight: 400;
                            width: 120px;
                        }
                    }
                }
            }
        }
    }

    & .ads {
        height: 480px;
        width: 100%;
        background-color:#fff;
        display: flex;
        justify-content: center;

        & > .ads-content {
            width: 581px;
            color:#000;

            & > .ads-main-text {
                font-size: 32px;
                font-weight: 700;
                text-align: center;
                margin-top:70px;
            }
            & > .ads-sub-text {
                margin-top:21px;
                font-size: 14px;
                text-align: center;

                & > p {
                    margin:0;
                }
            }
            & > .ads-img {
                margin-top: 32px;
            }
        }
    }
}
</style>
