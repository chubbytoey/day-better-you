<template>
    <div class="container">
        <div class="banner-container">
            <div class="overlay">
                <img src="../assets/images/banner.png">
                <div class="wrap">
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
                    <Banner />
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
                    <img src="../assets/images/image1.png">
                </div>
            </div>
        </div>

        <div class="popular-program-container">
            <div class="pop-block">
                <div class="popular-program-text">
                    โปรแกรมยอดนิยม
                </div>
                <div class="popular-program">
                    <Card
                        v-for="item in popularItems"
                        :key="item.id"
                        :data="item"
                    />
                </div>
                <div class="see-all-button">
                    <a-button class="custom-button" type="primary">
                        ดูทั้งหมด
                    </a-button>
                </div>
            </div>
        </div>

        <div class="bottom-banner-container">
            <img src="../assets/images/bottom-banner.png">
            <div class="bottom-banner-wrap">
                <div class="bottom-banner-text">
                    <List number="10+" description="โปรแกรมเปลี่ยน แปลงตัวเอง" />
                    <List number="100+" description="คำแนะนำจาก ผู้เชี่ยวชาญ" />
                    <List number="100+" description="สมาชิกผู้เข้าร่วม โปรแกรม" />
                </div>
            </div>
        </div>

        <div class="dowload-container">
            <div class="dowload-block">
                <div class="dowload-img">
                    <img src="../assets/images/Black-iPhone.png">
                    <Available />
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
                        <Dowload v-for="data in dowloadData" :key="data.id" :data="data" />
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
import Banner from '../components/BannerBlock'
import Available from '../components/Available'
import Dowload from '../components/DowloadButton'
import axios from 'axios'
export default {
    components: {
        Card, List, Banner, Available, Dowload
    },
    data () {
        return {
            popularItems: [],
            parIMG: [ require('../assets/images/par1.png'), require('../assets/images/par2.png'), require('../assets/images/par3.png'), require('../assets/images/par4.png'), require('../assets/images/par5.png'), require('../assets/images/par6.png'), require('../assets/images/par7.png'), require('../assets/images/par8.png'), require('../assets/images/par9.png'), require('../assets/images/par10.png'), require('../assets/images/par11.png'), require('../assets/images/par12.png'), require('../assets/images/par13.png'), require('../assets/images/par14.png'), require('../assets/images/par15.png'), require('../assets/images/par16.png'), require('../assets/images/par17.png'), require('../assets/images/par18.png'), require('../assets/images/par19.png'), require('../assets/images/par20.png'), require('../assets/images/par21.png') ],
            dowloadData: [
                {
                    id: 1,
                    img: require('../assets/images/apple-ic.png'),
                    subText: 'Dowload on the',
                    mainText: 'App Store'
                },
                {
                    id: 2,
                    img: require('../assets/images/playstore-ic.svg'),
                    subText: 'Get it on',
                    mainText: 'Google Play'
                }
            ]
        }
    },
    methods: {
        fetchData() {
            axios.get('https://seven-days-better-you-api.avalue.co.th/api/landing/program/list')
                .then(response => {
                    this.popularItems = response.data.programs
                })
        }
    }
    ,
    mounted() {
        this.fetchData()
        console.log(this.popularItems)
    }
}
</script>

<style lang="scss" scoped>
.container {
    & > .banner-container {
        width: 100%;
        height: 560px;
        position: relative;
        & > .overlay {
            width: 100%;
            height: 100%;
            background-color: $based-color;
            & > img {
                width: 100%;
                height: 100%;
                object-fit: cover;
            }
            & > .wrap {
                width: 100%;
                height: 100%;
                position: absolute;
                top: 0;
                & > .banner-text {
                    max-width: 1280px;
                    padding: 122px 0 0;
                    margin: 0 auto;
                    color:#fff;
                    text-align: center;
                    & > .main-text {
                        font-weight: 700;
                        font-size:40px;
                    }

                    & > .sub-text {
                        font-size: 0.875rem;
                        font-weight: 400;
                        width: 560px;
                        margin:20px auto 36px auto;
                        color: rgba(255,255,255, 0.65);
                    }
                }
            }
        }
    }

    & > .ads-container {
            height: 480px;
            max-width: 100%;
            background-color:#fff;
            display: flex;
            justify-content: center;

            & > .ads-content {
                width: 581px;

                & > .ads-main-text {
                    font-size: 32px;
                    font-weight: 700;
                    text-align: center;
                    margin-top:70px;
                    color: #000;
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
        min-height: 740px;
        padding: 80px 0;
        background-color: #F6F8FA;
        & > .pop-block {
            max-width: 1280px;
            width: 100%;
            margin: 0 auto;
            padding:0 56px;
            & > .popular-program-text {
                font-size:24px;
                font-weight: 700;
                color:#000;
                margin-bottom: 33px;
            }

            & > .popular-program {
                color: red;
                margin-bottom: 2.75rem;
                display: flex;
                justify-content: flex-start;
                /* flex-wrap: wrap; */
                overflow-x: auto;
                overflow-y: hidden;
                padding:16px 0;
            }
            & > .see-all-button {
                width: fit-content;
                margin:0 auto;
            }
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
        & > .bottom-banner-wrap {
            width: 100%;
            max-width: 1280px;
            height: 300px;
            position: absolute;
            display: flex;
            align-items: center;
            justify-content: center;
            & > .bottom-banner-text {
                width: 100%;
                max-width: 900px;
                color:#fff;
                display: flex;
                justify-content: flex-start;
                flex-wrap: wrap;
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
                    font-weight: 400;
                    text-align: center;
                }
            }
        }
    }
}
@media screen and (max-width: 800px) {
    .participation-block{
        width: 700px !important;
        height: 210px !important;
        & > .participation-img {
            grid-template-columns: repeat(7, 60px) !important;
            grid-template-rows: repeat(3, 60px) !important;
            & > .par-img{
            width: 60px !important;
            }
        }
    }
    .bottom-banner-text {
        justify-content: center !important;
    }
}
</style>
