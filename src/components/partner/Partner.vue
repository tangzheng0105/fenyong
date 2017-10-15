<template>
    <div>
        <my-header></my-header>
        
        <div>
            <div class="partner-list-item">
                <div class="partner-list-title">
                    <table width='100%'>
                        <tr>
                            <td>31群(我自己)</td>
                            <td style="text-align: right">查看他的下级>></td>                            
                        </tr>
                    </table>
                </div>
                <div class="partner-list-info">
                    <table width='100%'>
                        <tr>
                            <td>订单：0</td>
                            <td>他的预估：0.00</td>
                            <td>我的提成：0.00</td>
                        </tr>
                    </table>
                </div>
            </div>
        </div>
        <h4 class="partner-list-header">我的一级合伙人:</h4>
        <div class="partner-list">
            <div v-for="n in 30" class="partner-list-item">
                <div class="partner-list-title">
                    <table width='100%'>
                        <tr>
                            <td>31群</td>
                            <td style="text-align: right">查看他的下级>></td>                            
                        </tr>
                    </table>
                </div>
                <div class="partner-list-info">
                    <table width='100%'>
                        <tr>
                            <td>订单：0</td>
                            <td>他的预估：0.00</td>
                            <td>我的提成：0.00</td>
                        </tr>
                    </table>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import MyHeader from '../Header.vue'
export default {
    name: 'partner',
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
.partner-list {
    padding-bottom: 60px;
    font-size: 16px;
    color: #888;
}
.partner-list-item {
    margin-top: 4px;
    border: 1px solid #ccc;
    border-radius: 4px;
}
.partner-list-title {
    border-bottom: 1px solid #ccc;
}
.partner-list-item td {
    padding: 6px 6px;
}
.partner-list-header {
    padding-left: 10px;
}
</style>

