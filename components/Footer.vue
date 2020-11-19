<template>
    <div class="footer-container">
        <div class="footer-top">
            <div class="footer-description">
                <div class="footer-main">
                    7 DAYS BETTER YOU
                </div>
                <div class="footer-sub">
                    Simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s…
                </div>
            </div>
            <div class="footer-list">
                <div class="footer-web">
                    <div class="footer-main">
                        เว็ปไซต์
                    </div>
                    <div class="footer-sub">
                        <ul>
                            <li>หน้าแรก</li>
                            <li>โปรแกรม</li>
                            <li>ติดต่อเรา</li>
                        </ul>
                    </div>
                </div>
                <div class="footer-web">
                    <div class="footer-main">
                        อื่นๆ
                    </div>
                    <div class="footer-sub">
                        <ul>
                            <li>เข้าสู่ระบบ</li>
                            <li>เงื่อนไขการใช้งาน</li>
                            <li>นโนยายความเป็นส่วนตัว</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        <div class="footer-bottom">
            © 2020 All Rights Reserved, 7 DAYS BETTER YOU
        </div>
    </div>
</template>
<script>
export default {

}
</script>
<style lang="scss" scoped>
.footer-container {
        height: 350px;
        width: 100%;
        background-color: $based-color;
        color:#fff;
        display: flex;
        flex-direction: column;
        & > .footer-top {
            max-width: 1280px;
            width: 100%;
            display: flex;
            margin:0 auto;
            margin-top:63px;
            flex:1;
            justify-content: space-between;
            & > .footer-description {
                width: 360px;
                margin-left: 68px;
                & > .footer-main {
                    font-size: 16px;
                    font-weight: 700;
                }
                & >  .footer-sub {
                    font-size: 14px;
                    font-weight: 400;
                    opacity: 0.65;
                    margin-top:16px;
                }
            }
            & > .footer-list {
                display: flex;
                margin-right: 45px;
                & > .footer-web {
                    width: fit-content;
                    & > :first-child {
                        margin-right: 137px;
                    }
                    & > .footer-main {
                        font-size: 16px;
                        font-weight: 700;
                    }
                    & > .footer-sub {
                        margin-top:16px;
                        font-size: 14px;
                        font-weight: 400;
                        opacity: 0.65;
                        & > ul {
                            list-style: none;
                            padding: 0;
                            & > li {
                            margin-top:13px;
                            }
                        }
                    }
                }
            }
        }
        & > .footer-bottom {
            height: 56px;
            width: 100%;
            border-top:1px solid rgb(255,255,255,0.16);
            font-size: 12px;
            font-weight: 400;
            display: flex;
            align-items: center;
            justify-content: center;
        }

    }
</style>
