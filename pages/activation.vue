<template>
    <el-collapse v-model="activeNames" @change="handleChange">
        <el-collapse-item
            title="活性化関数"
            name="1"
            class="big bigbig bigbigbig"
        >
            <div>
                入力信号の総和を出力信号に変換する関数
            </div>
            <div>
                入力信号の総和がどのように活性化するのか決定する役割があります
            </div>
            <div>
                重み付き入力信号とバイアスの総和を計算し、それをaとします
            </div>
            <div>
                $$ a = b + w_1x_1 + w_2x_2$$
            </div>
            <div>
                aが活性化関数h()で変換されyが出力されます
            </div>
            <div>
                $$y = h(a)$$
            </div>
            <div>
                画像
            </div>
            <div>
                重み付き信号の和がaというニューロンになり、
                そして活性化関数h()によってyというニューロンに変換されます
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
