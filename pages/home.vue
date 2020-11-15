<template>
  <div class="container">
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
    </div>

    <div class="ads-container">
      <div class="ads-content">
        <div class="ads-main-text">
          เปลี่ยนเป็นคุณคนใหม่ใน 7 วัน
        </div>
        <div class="ads-sub-text">
          <p>เนื้อหาจำลองแบบเรียบๆ ที่ใช้กันในธุรกิจงานพิมพ์หรืองานเรียงพิมพ์</p>
          <p>มันได้กลายมาเป็นเนื้อหาจำลองมาตรฐานของธุรกิจดังกล่าวมาตั้งแต่ศตวรรษที่ 16</p>
        </div>
        <div class="ads-img">
          <img src="../assets/image1.png">
        </div>
      </div>
    </div>

    <div class="popular-program-container">
      <div class="popular-program-text">
        โปรแกรมยอดนิยม
      </div>
      <div class="popular-program">
        <Card
          v-for="item in popularItems"
          :key="item.id"
          :src="item.img"
          :main-message="item.mainMessage"
          :sub-message="item.subMessage"
          :price="item.price"
        />
      </div>
      <div class="see-all-button">
        <a-button class="custom-button" type="primary">
          ดูทั้งหมด
        </a-button>
      </div>
    </div>

    <div class="bottom-banner-container">
      <img src="../assets/bottom-banner.png">
      <div class="bottom-banner-text">
        <List number="10+" description="โปรแกรมเปลี่ยน แปลงตัวเอง" />
        <List number="100+" description="คำแนะนำจาก ผู้เชี่ยวชาญ" />
        <List number="100+" description="สมาชิกผู้เข้าร่วม โปรแกรม" />
      </div>
    </div>

    <div class="dowload-container">
      <div class="dowload-block">
        <div class="dowload-img">
          <img src="../assets/Black-iPhone.png">
          <div class="avaliable">
            <p class="avaliable-sub">
              avaliable
            </p>
            <p class="avaliable-main">
              now
            </p>
          </div>
        </div>
        <div class="dowload">
          <div class="dowload-main-text">
            ดาวน์โหลดแอพลิเคชั่นเพื่อการเปลี่ยนแปลงตัวเอง
          </div>
          <div class="dowload-sub-text">
            <p>เนื้อหาจำลองแบบเรียบๆ ที่ใช้กันในธุรกิจงานพิมพ์หรืองานเรียงพิมพ์</p>
            <p>มันได้กลายมาเป็นเนื้อหาจำลองมาตรฐานของธุรกิจดังกล่าวมาตั้งแต่ศตวร</p>
            <p>รษที่ 16 เมื่อเครื่องพิมพ์โนเนมเครื่องหนึ่งนำราง</p>
          </div>
          <div class="load-now">
            <a-button class="custom-button">
              <div class="button-img">
                <img src="../assets/apple-ic.png">
              </div>
              <div class="button-text">
                <p class="sub-load">
                  Dowload on the
                </p>
                <p class="main-load">
                  App Store
                </p>
              </div>
            </a-button>
            <a-button class="custom-button">
              <div class="button-img">
                <img src="../assets/playstore-ic.svg">
              </div>
              <div class="button-text">
                <p class="sub-load">
                  Get it on
                </p>
                <p class="main-load">
                  Google Play
                </p>
              </div>
            </a-button>
          </div>
        </div>
      </div>
    </div>

    <div class="participation-container">
      <div class="participation-block">
        <div class="participation-img">
          <div v-for="img in parIMG" :key="img.index" class="par-img">
            <img :src="img">
          </div>
        </div>
        <div class="participation-text">
          <p>ผู้เข้าร่วม</p>
          <p>กว่า 100 ราย</p>
          <a-button class="custom-button" type="primary">
            เข้าร่วมกับเรา
          </a-button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Card from '../components/Card'
import List from '../components/BannerList'
export default {
  components: {
    Card, List
  },
  data () {
    return {
      popularItems: [
        {
          id: 1,
          img: require('../assets/pop-pro.png'),
          mainMessage: 'สร้างความมั่นใจ',
          subMessage: 'เติมพลังความมั่นใจ ให้ทุกวันเป็นวันทีทรงพลัง',
          price: 'ฟรี'
        },
        {
          id: 2,
          img: require('../assets/pop-pro1.png'),
          mainMessage: 'สร้างความมั่นใจ',
          subMessage: 'เติมพลังความมั่นใจ ให้ทุกวันเป็นวันทีทรงพลัง',
          price: '300฿'
        },
        {
          id: 3,
          img: require('../assets/pop-pro2.png'),
          mainMessage: 'สร้างความมั่นใจ',
          subMessage: 'เติมพลังความมั่นใจ ให้ทุกวันเป็นวันทีทรงพลัง',
          price: '300฿'
        },
        {
          id: 4,
          img: require('../assets/pop-pro3.png'),
          mainMessage: 'สร้างความมั่นใจ',
          subMessage: 'เติมพลังความมั่นใจ ให้ทุกวันเป็นวันทีทรงพลัง',
          price: '300฿'
        }
      ],
      parIMG: [require('../assets/par1.png'), require('../assets/par2.png'), require('../assets/par3.png'), require('../assets/par4.png'), require('../assets/par5.png'), require('../assets/par6.png'), require('../assets/par7.png'), require('../assets/par8.png'), require('../assets/par9.png'), require('../assets/par10.png'), require('../assets/par11.png'), require('../assets/par12.png'), require('../assets/par13.png'), require('../assets/par14.png'), require('../assets/par15.png'), require('../assets/par16.png'), require('../assets/par17.png'), require('../assets/par18.png'), require('../assets/par19.png'), require('../assets/par20.png'), require('../assets/par21.png')]
    }
  }
}
</script>

<style lang="scss" scoped>
.container {
    & > .banner-container {
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

    }

    & > .ads-container {
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

    & > .popular-program-container {
        width: 100%;
        height: 740px;
        padding-top: 80px;
        background-color: #F6F8FA;

        & > .popular-program-text {
            margin-left: 56px;
            font-size:24px;
            font-weight: 700;
            color:#000;
            margin-bottom: 33px;
        }

        & > .popular-program {
            color: red;
            padding:0 56px;
            margin-bottom: 2.75rem;
            display: flex;
            justify-content: space-around;
        }

        & > .see-all-button {
            width: fit-content;
            margin:0 auto;
        }
    }

    & > .bottom-banner-container {
        background-color: $based-color;
        height: 300px;
        width: 100%;
        display: flex;
        align-items: center;
        justify-content: center;

        & > img {
            width: 100%;
            height: 300px;
        }
        & > .bottom-banner-text {
            width: 900px;
            position: absolute;
            color:#fff;
            display: flex;
            & > :first-child {
                margin-right: 90px;
            }
            & > :last-child {
                margin-left: 90px;
            }
        }
    }

    & > .dowload-container {
        height: 622px;
        width: 100%;
        background-color: #fff;
        overflow: hidden;
        display: flex;
        justify-content: center;
        & > .dowload-block {
            width: 905px;
            height: 795px;
            display: flex;
            margin-top:100px;
            & > .dowload-img {
                flex:1;
                position: relative;
                & > img {
                    -webkit-filter: drop-shadow(0px 1px 4px rgba(0, 0, 0, 0.2));
                    filter: drop-shadow(0px 1px 4px rgba(0, 0, 0, 0.2));
                }
                & > .avaliable {
                    width: 127px;
                    height: 127px;
                    border-radius:50% ;
                    background-color: #062A3A;
                    border:none;
                    outline: none;
                    position: absolute;
                    top:42px;
                    left:298px;
                    color:#fff;
                    display: flex;
                    flex-direction:column;
                    justify-content: center;
                    align-items: center;
                    & > p {
                        margin:0;
                    }
                    & > .avaliable-main {
                        font-size:32px;
                        margin-top:-10px;
                        text-transform: uppercase;
                        font-weight: 700;
                        letter-spacing: 2px;
                    }
                    & > .avaliable-sub {
                        font-size: 16px;
                        text-transform: capitalize;
                    }
                }
            }
            & > .dowload {
                display: flex;
                flex-direction: column;
                flex:1;
                padding-top:84px;
                & > .dowload-main-text {
                    font-size: 32px;
                    font-weight: 700;
                    color:#000;
                }
                & > .dowload-sub-text {
                    font-size:14px;
                    font-weight: 400;
                    margin-top:16px;
                    & > p {
                        margin: 0 !important;
                    }
                }
                & > .load-now {
                    display: flex;
                    margin-top:47px;
                    & > button {
                        background-color: #000;
                        border: #A9AAA9 1px solid;
                        width: 186px;
                        height: 54px;
                        display: flex;
                        border-radius: 10px;
                        & > .button-text {
                            width: 140px;
                            height: 100%;
                            padding-left: 10px;
                            flex:1;
                            display: flex;
                            flex-direction: column;
                            align-items: flex-start;
                            justify-content: center;
                            & > p {
                                margin:0;
                            }
                            & > .main-load {
                                font-size: 22px;
                                margin-top:-7px;
                            }
                        }
                        & > .button-img {
                            height: 100%;
                            display: flex;
                            align-items: center;
                            justify-content: center;
                            & > img {
                                margin-top:-5px;
                            }
                        }
                    }
                }
            }
        }
    }

    & > .participation-container {
        width: 100%;
        height: 472px;
        background-color: #F6F8FA;
        display: flex;
        justify-content: center;
        align-items: center;
        & > .participation-block {
            width: 960px;
            height: 272px;
            display: flex;
            border-radius: 10px;
            box-shadow:0 4px 8px 0 rgba(0, 0, 0, 0.2);
            & > .participation-img {
                background-color: #fff;
                display: grid;
                grid-template-columns: repeat(7,80px);
                grid-template-rows: repeat(3,80px);
                grid-column-gap: 8px;
                grid-row-gap: 8px;
                padding: 8px;
                border-radius:10px 0 0 10px ;
                & > .par-img {
                    width: 80px;
                    height: 80px;
                    & > img {
                        width: 100%;
                    }
                }
            }
            & > .participation-text {
                width: 336px;
                flex:1;
                background-color: #062A3A;
                color:#fff;
                display: flex;
                justify-content: center;
                align-items: center;
                flex-direction: column;
                border-radius: 0 10px 10px 0;
                & > button {
                    color:#fff ;
                    text-shadow: none;
                    background-color: rgb(255,255,255,0.45);
                    margin-top:41px;
                }
                & > p {
                    margin: 0;
                    font-size: 26px;
                    font-weight: 700;
                    text-align: center;
                }
            }
        }
    }

}
</style>
