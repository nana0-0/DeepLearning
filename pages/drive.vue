<template>
    <el-collapse v-model="activeNames" @change="handleChange">
        <el-collapse-item
            title="データ駆動"
            name="1"
            class="big bigbig bigbigbig"
        >
            <div>
                画像から特徴量を抽出して、その特徴量のパターンを機械学習の技術で学習
            </div>
        </el-collapse-item>
        <el-collapse-item
            title="特徴量とは"
            name="2"
            class="big bigbig bigbigbig"
        >
            <div>
                入力データ(入力画像)から本質的なデータ(重要なデータ)を的確に抽出できるように設計された変換器を指す
            </div>
            <div>
                画像の特徴量は通常ベクトルとして記述される
            </div>
        </el-collapse-item>
        <el-collapse-item
            title="有名な特徴量"
            name="3"
            class="big bigbig bigbigbig"
        >
            <div>
                SIFT 
            </div>
            <div>
                SURF 
            </div>
            <div>
                 HOG
            </div>
            <div>
                 これらを使って画像データをベクトルに変換する。
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
