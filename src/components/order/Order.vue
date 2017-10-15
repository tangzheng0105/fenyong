<template>
    <div class="order">
        <my-header></my-header>

        <div class="search">
            <mt-search v-model="value" cancel-text="取消" placeholder="订单编号/宝贝标题">
            </mt-search>
        </div>
        <div class="order-list">
            <div class="order-list-item" v-for="item in orderList">
                <div class="order-list-title">衣品天成 2017秋季新款男士休闲裤男 裤子男装韩版潮流直筒长裤秋</div>
                <div class="order-list-body">
                    <table width='100%'>
                        <tr>
                            <td>订单：73391514579772289</td>
                            <td>付款金额：122.24</td>
                        </tr>
                        <tr>
                            <td>订单状态：订单付款</td>
                            <td> 工资：4.49</td>
                        </tr>
                        <tr>
                            <td>下单时间：2017-10-13 09:11:38</td>
                            <td> 工资状态：工资未结</td>
                        </tr>
                    </table>
                </div>
            </div>
        </div>

    </div>
</template>

<script>
import Vue from 'vue'
import MyHeader from '../Header.vue'
import { Search, Cell } from 'mint-ui';

Vue.component(Search.name, Search);
Vue.component(Cell.name, Cell);
export default {
    name: 'index',
    data() {
        return {
            value: '',
            orderList: [
                { title: 'aa', value: 'bb' },
                { title: 'aa', value: 'bb' },
                { title: 'aa', value: 'bb' },
                { title: 'aa', value: 'bb' },
                { title: 'aa', value: 'bb' }
            ]
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
.search {
    margin-top: 10px;
    height: 53px;
    overflow: hidden;
}

.order-list {
    width: 96%;
    padding: 6px;
    font-size: 12px;
    padding-bottom: 60px;
}

.order-list-item {
    background-color: #fff;
    margin-top: 4px;
    border-radius: 4px;
    border: 1px solid #ccc;
    padding: 4px;
}

.order-list-title {
    width: 100%;
    border-bottom: 1px solid #ccc;
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-line-clamp: 1;
    overflow: hidden;
    padding: 2px;
}

.order-list-body {}
</style>

