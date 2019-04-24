<template>
    <div class="footerbar">
        <div v-for="item in navItem">
            <div>
                <img src="../assets/logo.png" style="width: 10px;height: 10px;display: block">
            </div>
            <span>
                {{item.name}}
            </span>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'MyFooterBar',
        data() {
            return {
                navItem:[{name:'首页',icon:''},{name:'附近',icon:''},{name:'逛一逛',icon:''},{name:'订单',icon:''},{name:'我的',icon:''}]
            }
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<!--npm install -D sass-loader node-sass 加载css预编译器-->
<style scoped lang="scss">
.footerbar{
    position: fixed;
    bottom: 0;
    width: 100%;
    height: 40px;
    border-top: rgba(217, 217, 217, 1) solid 1px;
    display: flex;
    justify-content: center;
    align-items: center;
    >div{
        flex: 1;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        max-width: 168px;
        font-size: 12px;
        font-weight: 400;
        >div{
            display: flex;
            width: 100%;
            align-items: center;
            justify-content: center;
        }
    }
}
</style>
