<template>
    <el-collapse v-model="activeNames" @change="handleChange">
        <el-collapse-item title="重み" name="1" class="big bigbig bigbigbig">
            <div>
                重みはその値が大きければ大きいほど大きな信号が流れる
            </div>
            <div>
                →信号の流れにくさをコントロールする
            </div>
            <div>
                入力信号への重要度をコントロールするパラメータ
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
