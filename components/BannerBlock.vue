<template>
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
                    <img src="../assets/images/ic-banner1.svg">
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
                    <img src="../assets/images/ic-banner2.svg">
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
                    <img src="../assets/images/ic-banner3.svg">
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {

}
</script>
<style lang="scss" scoped>
.banner-block-container {
    width: 100%;
    /* height: 127px;
    display: flex;
    justify-content: center; */
    position: absolute;
    bottom:0;
    & > .banner-block {
        /* position: absolute; */
        max-width: 960px;
        width: 100%;
        margin: 0 auto;
        height: 127px;
        background-color: rgb(255,255,255,0.3);
        /* bottom: 0; */
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
</style>
