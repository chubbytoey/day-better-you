<template>
    <div class="topbar-container">
        <div class="block">
            <div class="logo-container">
                <div class="logo-icon">
                    <img src="../assets/images/logo.svg">
                </div>
                <label>day better you</label>
            </div>
            <div class="menu-container">
                <div class="menu">
                    <nuxt-link to="/" class="list active">
                        หน้าแรก
                    </nuxt-link>
                    <nuxt-link to="/" class="list">
                        โปรแกรม
                    </nuxt-link>
                    <nuxt-link to="/" class="list">
                        ติดต่อเรา
                    </nuxt-link>
                </div>
                <a-divider class="line-divider" type="vertical" />
                <a-button class="custom-button" type="primary">
                    เริ่มโปรแกรม
                </a-button>
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>

.topbar-container {
  width: 100%;
  background-color: #fff;
  border-top: $based-color 4px solid;
    & > .block {
        max-width: 1280px;
        min-height: 64px;
        margin: 0 auto;
        padding: 0 56px;
        display: flex;
        flex-wrap: wrap;
        align-items: center;
        justify-content: space-between;
        & > .logo-container {
            text-transform: uppercase;
            display: flex;
            justify-content: center;
            align-items: center;
            & > .logo-icon {
                width: 32px;
                height: 32px;
                margin-right:10px;
                & > img {
                    width: 100%;
                    height: 100%;
                }
            }
            & > label {
                font-size: 1.25rem;
                font-weight: 700;
                color: $based-color;
            }
        }

        & > .menu-container {
            display: flex;
            font-size: 0.875rem;
            align-items: center;
            & > .menu {
                padding:10px;
                display: flex;
                color:#000;
                height: 64px;
                align-items: center;

                & > .list {
                    padding: 0 19px;
                }
                & > a {
                    color:$based-color;
                }
                & > .active {
                    font-weight: bold;
                }
            }

            & > .line-divider {
                height: 32px;
                margin-right: 24px;
            }

        }
    }
}
</style>
