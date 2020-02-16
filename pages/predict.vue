<template>
    <el-collapse v-model="activeNames" @change="handleChange">
        <el-collapse-item
            title="推論処理"
            name="1"
            class="big bigbig bigbigbig"
        >
            <div>
                ニューラルネットワークの順方向伝播という
            </div>
            <div>
                ニューラルネットワークを使って問題を解く
            </div>
            <div>
                学習と推論によって行われる
                訓練データを使って重みパラメータの学習を行い
                推論時には先に学習したパラメータを使って 入力データの分類を行う
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
