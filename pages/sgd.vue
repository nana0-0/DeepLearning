<template>
    <el-collapse v-model="activeNames" @change="handleChange">
        <el-collapse-item
            title="勾配"
            name="1"
            class="big bigbig bigbigbig"
        >
            <div>
                勾配の示す方向は各場所において関数の値をもっとも減らす方向
            </div>
        </el-collapse-item>
        <el-collapse-item
            title="勾配法"
            name="2"
            class="big bigbig bigbigbig"
        >
            <div>
                学習の際に最適なパラメータを探索する
            </div>
            <div>
                最適なパラメータというのは損失関数が最小値を取るときのパラメータの値(重みとバイアス)
            </div>
        </el-collapse-item>
        <el-collapse-item
            title="ニューラルネットワーク"
            name="3"
            class="big bigbig bigbigbig"
        >
            <div>
                ニューラルネットワークの勾配は重みパラメータに関する損失関数の勾配です
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
