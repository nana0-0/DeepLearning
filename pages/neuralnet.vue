<template>
    <el-collapse v-model="activeNames" @change="handleChange">
        <el-collapse-item
            title="ニューラルネットワーク"
            name="1"
            class="big bigbig bigbigbig"
        >
            <div>
                データから学習できる
            </div>
            <div>
                データから学習できるとは、重みパラメータの値をデータから自動で決定できるということです
            </div>
        </el-collapse-item>
        <el-collapse-item
            title="パーセプトロンの働きの確認"
            name="2"
            class="big bigbig bigbigbig"
        >
            <div>
                b
                バイアスはニューロンの発火のしやすさをコントロールするパラメータ
            </div>
            <div>
                w 各信号の重要性をコントロールするパラメータ
            </div>
            <div>
                パーセプトロンの動作は入力xに重みが乗算され次のニューロンに送信されます
            </div>
            <div>
                次のニューロンではそれらの重み付けされた信号の和が計算され、その和が0を超えたら1を出力しそうでなければ0を出力します
            </div>
            <div>
                $$ \begin{equation} y= \left \{ \begin{array}{l} 0　(b + w_1x_1
                + w_2x_2 \leqq 0) \\ 1　(b + w_1x_1 + w_2x_2> 0) \end{array}
                \right. \end{equation} $$
            </div>
            <div>
                ここで0を超えたら1を出力しそうでなければ0を出力するという場合わけの動作を関数であらわします
            </div>
            <div>
                $$y= h(b+w_1x_1+w_2x_2)$$
            </div>
            <div>
                $$ \begin{equation} h(x)=\left\{ \begin{array}{1} 0　(x\leqq 0)
                \\ 1　(x> 0) \end{array} \right. \end{equation} $$
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
