<template>
    <el-collapse v-model="activeNames" @change="handleChange">
        <el-collapse-item
            title="バイアス"
            name="1"
            class="big bigbig bigbigbig"
        >
            <div>
                bをバイアスと呼びます
            </div>
            <div>
                →出力信号が1を出力する度合いをコントロール
            </div>
            <div>
                バイアスは発火のしやすさをコントロールするパラメータ
            </div>
            <div>
                $$ \begin{equation} y= \left \{ \begin{array}{l} 0　(b + w_1x_1
                + w_2x_2 \leqq 0) \\ 1　(b + w_1x_1 + w_2x_2> 0) \end{array}
                \right. \end{equation} $$
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
