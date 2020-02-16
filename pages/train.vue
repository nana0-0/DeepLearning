<template>
    <el-collapse v-model="activeNames" @change="handleChange">
        <el-collapse-item
            title="学習"
            name="1"
            class="big bigbig bigbigbig"
        >
            <div>
                訓練データから適切な重みパラメータをの値を自動で獲得すること
            </div>
            <div>
                損失関数を基準として、その値がもっとも小さくなる重みパラメータを探し出すということが学習の目的
            </div>
        </el-collapse-item>
    </el-collapse>
</template>
<script>
export default {
    data() {
        return {
            activeNames: ['1']
        }
    },
    methods: {
        handleChange(val) {
            console.log(val)
        }
    }
}
</script>

<style scoped>
.big .bigbig .bigbigbig {
    font-size: 3em;
}
</style>
