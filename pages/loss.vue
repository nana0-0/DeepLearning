<template>
    <el-collapse v-model="activeNames" @change="handleChange">
        <el-collapse-item
            title="損失関数"
            name="1"
            class="big bigbig bigbigbig"
        >
            <div>
                学習を行えるようにするための「指標」
            </div>
        </el-collapse-item>
        <el-collapse-item
            title="出来るだけ小さな損失関数の値を探し出す手法"
            name="2"
            class="big bigbig bigbigbig"
        >
            <div>
                勾配法と呼ばれる、関数の傾きを使った手法
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
