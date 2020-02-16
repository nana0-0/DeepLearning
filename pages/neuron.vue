<template>
    <el-collapse v-model="activeNames" @change="handleChange">
        <el-collapse-item
            title="ニューロン"
            name="1"
            class="big bigbig bigbigbig"
        >
            <div>
                ニューロンに送られる際にそれぞれに固有の重みが乗算される
            </div>
            <div>
                $$(w_1x_1,w_2x_2)$$
            </div>
        </el-collapse-item>
        <el-collapse-item
            title="ニューロンの発火"
            name="2"
            class="big bigbig bigbigbig"
        >
            <div>
                ニューロンでは送られてきた信号の総和が計算される
            </div>
            <div>
                総和がある限界値を超えた場合のみ1を出力
            </div>
        </el-collapse-item>
        <el-collapse-item title="閾値" name="3" class="big bigbig bigbigbig">
            <div>
                ある限界値のことを閾値と呼びθであらわす
            </div>
            <div>
                $$ \begin{equation} y= \left \{ \begin{array}{l} 0　(w_1x_1 +
                w_2x_2 \leqq \theta ) \\ 1　(w_1x_1 + w_2x_2> \theta)
                \end{array} \right. \end{equation} $$
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
