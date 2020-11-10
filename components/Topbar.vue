<template>
  <div class="topbar-container">
    <div class="logo-container">
      <div class="logo-icon">
        <img src='../assets/logo.svg'>
      </div>
      <label>day better you</label>
    </div>

    <div class="menu-container">
      <div class="menu">
        <div class="list"><b>หน้าแรก</b></div>
        <div class="list">โปรแกรม</div>
        <div class="list">ติดต่อเรา</div>
      </div>
      <a-divider class="line-divider" type="vertical" />
      <a-button class="custom-button" type="primary">เริ่มโปรแกรม</a-button>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>

.topbar-container {
  border-top: $based-color 4px solid;
  width: 100%;
  color:#fff;
  background-color: #fff;
  height: 64px;
  display: flex;
  font-size: 14px;
  justify-content: space-between;
  color: $based-color;
  padding:0 55px;

/* &.red {
    background-color:red;
} */
    & > .logo-container {
        text-transform: uppercase;
        display: flex;
        width: 210px;
        font-weight: 700;
        justify-content: center;
        align-items: center;
        font-size: 20px;

        & > .logo-icon {
            width: 32px;
            height: 32px;

            & > img {
              width: 100%;
            }
        }

        & > label {
            padding-left:10px;
        }
    }

    & > .menu-container {
        display: flex;
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
        }

        & > .line-divider {
            height: 32px;
            margin-right: 24px;
        }

    }
}
</style>
