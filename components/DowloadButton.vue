<template>
    <button class="custom-button">
        <div class="button-img">
            <img :src="data.img">
        </div>
        <div class="button-text">
            <p class="sub-load">
                {{ data.subText }}
            </p>
            <p class="main-load">
                {{ data.mainText }}
            </p>
        </div>
    </button>
</template>
<script>
export default {
    props: {
        data: {
            type: Object,
            default: null
        }
    }
}
</script>
<style lang="scss" scoped>
button {
    background-color: #000;
    border: #A9AAA9 1px solid;
    width: 186px;
    height: 54px;
    display: flex;
    border-radius: 10px;
    align-items: center;
    margin-right: 12px;
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
            font-size: 20px;
            margin-top:-7px;
        }
        & > .sub-load {
            font-size:14px;
        }
    }
    & > .button-img {
        height: 100%;
        display: flex;
        align-items: center;
        justify-content: center;
        padding: 10px;
        & > img {
            margin-top:-5px;
        }
    }
}

</style>
