<template>
  <div class="container">
    <a-card hoverable style="width: 240px">
      <img
        slot="cover"
        alt="example"
        :src="src"
      >
      <a-card-meta :title="mainMessage">
        <template slot="description">
          <p>{{ subMessage }}</p>
          <p class="price">
            {{ price }}
          </p>
        </template>
      </a-card-meta>
    </a-card>
    <div class="gradient-overlay" />
  </div>
</template>
<script>
export default {
  props: {
    mainMessage: {
      type: String,
      default: ' '
    },
    subMessage: {
      type: String,
      default: ' '
    },
    price: {
      type: String,
      default: ''
    },
    src: {
      type: String,
      default: ' '
    }
  }
}
</script>
<style lang="scss" scoped>
.container{
    position: relative;
    .ant-card {
        color:darkblue;
        width: 280px !important;
        height: 416px !important;
        border-radius: 15px;
        border:none;
        box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.1);

        & > .ant-card-cover img {
            width: 280px;
            height: 280px;
            border-radius: 15px 15px 0 0;
        }

        & > .ant-card-body {
            background-color: red !important;

            & > .ant-card-meta .ant-card-meta-detail .ant-card-meta-description .price {
                color:#0AC775;
                font-size: 20px;
                font-weight: 700;
                margin-top:-10px;
            }
        }
    }
    & > .gradient-overlay {
        background-image: linear-gradient(to bottom, transparent, rgba(255,255,255));
        width: 280px;
        height: 50px;
        position: absolute;
        bottom:0;
        margin-bottom: 135px;
    }
}
</style>
