<template>
    <div class="container">
        <div>
            <logo />
            <h1 class="title">
                Neural Style Transfer
            </h1>
            <h2 class="subtitle">
                課題研究
            </h2>
            <div class="links">
                <nuxt-link to="/perceptron" class="button--green">
                    Deep Learning
                </nuxt-link>
                <a href="#" class="button--grey">
                    Neural Style Transfer
                </a>
            </div>
        </div>
    </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
    layout: 'home',
    components: {
        Logo
    }
}
</script>

<style>
.container {
    margin: 0 auto;
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
}

.title {
    font-family: 'Quicksand', 'Source Sans Pro', -apple-system,
        BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial,
        sans-serif;
    display: block;
    font-weight: 300;
    font-size: 100px;
    color: #35495e;
    letter-spacing: 1px;
}

.subtitle {
    font-weight: 300;
    font-size: 42px;
    color: #526488;
    word-spacing: 5px;
    padding-bottom: 15px;
}

.links {
    padding-top: 15px;
}

.button--green {
    display: inline-block;
    border-radius: 4px;
    border: 1px solid #3b8070;
    color: #3b8070;
    text-decoration: none;
    padding: 10px 30px;
}

.button--green:hover {
    color: #fff;
    background-color: #3b8070;
}

.button--grey {
    display: inline-block;
    border-radius: 4px;
    border: 1px solid #35495e;
    color: #35495e;
    text-decoration: none;
    padding: 10px 30px;
    margin-left: 15px;
}

.button--grey:hover {
    color: #fff;
    background-color: #35495e;
}
</style>
