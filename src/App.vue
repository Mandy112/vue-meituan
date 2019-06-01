<template>
    <div id="app">
    123456
        <MyFooterBar></MyFooterBar>
    </div>
</template>

<script>
    import MyFooterBar from './components/MyFooterBar.vue'

    export default {
        name: 'app',
        components:{
            MyFooterBar
        }
    }
</script>

<style>
    #app {
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
    }
    *{
        margin: 0;
        padding: 0;
    }
</style>
