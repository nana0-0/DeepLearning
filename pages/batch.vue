<template>
    <el-collapse v-model="activeNames" @change="handleChange">
        <el-collapse-item
            title="バッチ処理"
            name="1"
            class="big bigbig bigbigbig"
        >
            <div>
                多次元配列の対応する次元の要素数を一致させる
            </div>
            <div>
                バッチ処理によって一枚あたりの処理時間を大幅に短縮できる
            </div>
            <div>
                入力データのまとまりのことをバッチといい、バッチ単位で推論処理を行うことで計算を高速に行うことができる
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
