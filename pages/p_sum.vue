<template>
    <el-collapse v-model="activeNames" @change="handleChange">
        <el-collapse-item
            title="結局パーセプトロンって？"
            name="1"
            class="big bigbig bigbigbig"
        >
            <div>
                入力信号に重みが乗算された値とバイアスの和が計算される
            </div>
            <div>
                その値が閾値を上回っていれば1を出力する
            </div>
            <div>
                $$ \begin{equation} y= \left \{ \begin{array}{l} 0　(b + w_1x_1
                + w_2x_2 \leqq 0) \\ 1　(b + w_1x_1 + w_2x_2> 0) \end{array}
                \right. \end{equation} $$
            </div>
        </el-collapse-item>
        <el-collapse-item
            title="そもそも学習とは"
            name="2"
            class="big bigbig bigbigbig"
        >
            <div>
                学習とは適切なパラメータを決める作業である
            </div>
            <div>
                人が行う作業はパーセプトロンの構造(モデル)を考えコンピューターに学習データを与えることである
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
