<template>
    <el-collapse v-model="activeNames" @change="handleChange">
        <el-collapse-item
            title="パーセプトロン"
            name="1"
            class="big bigbig bigbigbig"
        >
            <div>
                複数の信号を受け取り一つの信号を出力する
            </div>
            <div>
                →情報の流れ
            </div>
            <div>
                →流すか流さないか(0か1)
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
