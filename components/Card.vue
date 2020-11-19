<template>
    <div class="container">
        <a-card
            class="card-block"
            hoverable
            style="width: 240px"
        >
            <template slot="cover">
                <img
                    alt="example"
                    :src="data.coverPath"
                >
                <div class="gradient-overlay" />
            </template>
            <a-card-meta :title="data.name">
                <template slot="description">
                    <p class="shortDescrip">
                        {{ data.shortDesc }}
                    </p>
                    <p class="price" v-if="data.price != 0">
                        {{ data.price }} ฿
                    </p>
                    <p class="price" v-else>
                        ฟรี
                    </p>
                </template>
            </a-card-meta>
        </a-card>
    </div>
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
.container {
    position: relative;
    margin-right: 16px;
    &:last-child {
        margin: 0;
    }
}
</style>
