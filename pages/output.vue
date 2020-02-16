<template>
    <el-collapse v-model="activeNames" @change="handleChange">
        <el-collapse-item title="出力層" name="1" class="big bigbig bigbigbig">
            <div>
                分類問題では出力層のニューロンの数を分類するクラス数に設定する
            </div>
        </el-collapse-item>
        <el-collapse-item
            title="ソフトマックス"
            name="2"
            class="big bigbig bigbigbig"
            ><div>
                分類問題
            </div>
            <div>
                オーバーフローに関する問題
            </div>
            <div>
                指数関数の計算が容易に大きくなる
            </div>
            <div>
                定数を足しても引いても結果は変わらない
            </div>
            <div>
                オーバーフロー対策として入力信号の最大値を用いる(最大値を引く)
            </div>
            <div>
                出力が0から1.0の実数になる
            </div>
            <div>
                ソフトマックス関数の総和は1になる
            </div>
            <div>
                出力を確率として解釈できる
            </div>
            <div>統計的な対応ができる</div>
            <div>各要素の大小関係は変わらない</div>
            <div>指数関数y＝exp(x)のが単調増加する関数であゆことに起因する</div>
            <div>
                ニューラルネットワークのクラス分類では
                出力の一番大きいニューロンに相当するクラスだけを認識結果とする
            </div>
        </el-collapse-item>
        <el-collapse-item title="恒等関数" name="3" class="big bigbig bigbigbig"
            ><div>
                回帰問題
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
