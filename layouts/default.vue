<template>
    <div>
        <el-container style="height: 100%">
            <el-aside
                width="360px"
                style="background-color: rgb(238, 241, 246)"
            >
                <el-menu :default-openeds="['1', '3']">
                    <el-submenu index="1">
                        <template slot="title">
                            <i class="el-icon-share"> </i>
                            パーセプトロン
                        </template>
                        <el-menu-item-group>
                            <template slot="title">概要</template>
                            <el-menu-item index="1-1-2">
                                <nuxt-link to="/perceptron">
                                    パーセプトロン
                                </nuxt-link>
                            </el-menu-item>
                            <el-menu-item index="1-1-2">
                                <nuxt-link to="/neuron">
                                    ニューロン
                                </nuxt-link>
                            </el-menu-item>
                            <el-menu-item index="1-1-3">
                                <nuxt-link to="/weight">
                                    重み
                                </nuxt-link>
                            </el-menu-item>
                            <el-menu-item index="1-1-4">
                                <nuxt-link to="/bias">
                                    バイアス
                                </nuxt-link>
                            </el-menu-item>
                            <el-menu-item index="1-1-5">
                                <nuxt-link to="/p_sum">
                                    まとめ
                                </nuxt-link>
                            </el-menu-item>
                        </el-menu-item-group>
                    </el-submenu>

                    <el-submenu index="2">
                        <template slot="title">
                            <i class="el-icon-monitor"> </i>
                            ニューラルネットワーク
                        </template>
                        <el-menu-item-group>
                            <template slot="title">概要</template>
                            <el-menu-item index="2-1"
                                ><nuxt-link to="/neuralnet"
                                    >ニューラルネットワーク</nuxt-link
                                ></el-menu-item
                            >
                            <el-menu-item index="2-2"
                                ><nuxt-link to="/activation"
                                    >活性化関数(activation function)</nuxt-link
                                >
                            </el-menu-item>
                            <el-menu-item index="2-3"
                                ><nuxt-link to="/output">出力層</nuxt-link>
                            </el-menu-item>
                            <el-menu-item index="2-3"
                                ><nuxt-link to="/predict">推論処理</nuxt-link>
                            </el-menu-item>
                            <el-menu-item index="2-3"
                                ><nuxt-link to="/batch">バッチ処理</nuxt-link>
                            </el-menu-item>
                            <el-menu-item index="2-3"
                                ><nuxt-link to="/train">学習</nuxt-link>
                            </el-menu-item>
                            <el-menu-item index="2-3"
                                ><nuxt-link to="/drive">データ駆動</nuxt-link>
                            </el-menu-item>
                            <el-menu-item index="2-3"
                                ><nuxt-link to="/loss">損失関数</nuxt-link>
                            </el-menu-item>
                            <el-menu-item index="2-3"
                                ><nuxt-link to="/sgd">勾配</nuxt-link>
                            </el-menu-item>
                        </el-menu-item-group>
                    </el-submenu>
                    <el-submenu index="3">
                        <template slot="title"
                            ><i class="el-icon-setting"></i
                            >学習アルゴリズム</template
                        >
                        <el-menu-item-group>
                            <template slot="title">概要</template>
                        </el-menu-item-group>
                    </el-submenu>
                </el-menu>
            </el-aside>
            <el-main>
                <nuxt />
            </el-main>
        </el-container>
    </div>
</template>

<style scoped>
html {
    font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
        'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
    font-size: 16px;
    word-spacing: 1px;
    -ms-text-size-adjust: 100%;
    -webkit-text-size-adjust: 100%;
    -moz-osx-font-smoothing: grayscale;
    -webkit-font-smoothing: antialiased;
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

/* .el-container {
    margin: 0;
    padding: 0;
    border: none;
}*/

a {
    text-decoration: none;
    color: black;
}

a:hover {
    color: rgb(77, 158, 224);
}

*,
*:before,
*:after {
    box-sizing: border-box;
    margin: 0;
}
</style>
