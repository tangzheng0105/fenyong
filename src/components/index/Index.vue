<template>
    <div>
        <my-header></my-header>
        <div class="body">
            <div class="body-item">
                <div>个人订单</div>
                <div>0.00</div>
            </div>
            <div style="background-color: #BF3030" class="body-item">
                <div>个人预估</div>
                <div>0.00</div>
            </div>
            <div style="background-color: #FFB273" class="body-item">
                <div>合伙人订单</div>
                <div>0.00</div>
            </div>
            <div style="background-color: #33CCCC" class="body-item">
                <div>合伙人提成</div>
                <div>0.00</div>
            </div>
            <div style="background-color: #FF7373" class="body-item">
                <div>余额</div>
                <div>0.00</div>
            </div>
            <div style="background-color: #009999" class="body-item">
                <div>已提现</div>
                <div>0.00</div>
            </div>
        </div>
        <button class="widthdraw">我要提现</button>
    </div>
</template>

<script>
import MyHeader from '../Header.vue'
export default {
    name: 'index',
    data() {
        return {
        }
    },
    methods: {
    },
    components: {
        MyHeader
    }
}
</script>

<style scoped>
.body {
    padding-top: 10px;
    width: 100%;
    overflow: hidden;
}

.body-item {
    width: 46%;
    margin: 4px 2%;
    float: left;
    background-color: deepskyblue;
    border-radius: 10px;
    height: 60px;
    text-align: center;
    font-size: 14px;
    color: #fff;
}

.body-item div {
    height: 50%;
    line-height: 30px;
}
.widthdraw {
    width: 90%;
    background-color: #FF0000;
    color: #fff;
    font-size: 16px;
    margin: 0 auto;
    display: block;
    margin-top: 180px;
    border: none;
    height: 40px;
    border-radius: 6px;
}
</style>

