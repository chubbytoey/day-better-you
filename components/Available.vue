<template>
    <div class="avaliable">
        <p class="avaliable-sub">
            available
        </p>
        <p class="avaliable-main">
            now
        </p>
    </div>
</template>
<script>
export default {

}
</script>
<style lang="scss" scoped>
.avaliable {
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
</style>
