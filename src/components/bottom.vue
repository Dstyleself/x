<template>
    <div class="bottomRoot">
        <ul>
            <li>
                <span>历史</span>
            </li>
            <li>
                <span>订阅</span>
            </li>
            <li>
                <span>我的</span>
            </li>
            <div class="clear"></div>
        </ul>
    </div>
</template>
<script>

    export default{

    }
</script>

<style>
    .bottomRoot{
        position: fixed;
        bottom: 0;
        background: #fff;
        right: 0;
        left: 0;
        border-top: 1px solid #f5f5f5;
        height: 35px;
        line-height: 35px;
        font-size: 12px;
    }
    .bottomRoot ul{
        list-style-type:none;
        width: 100%;
        padding-left: 0;
    }
    .bottomRoot ul li{
        float: left;
        display: inline-block;
        width: 33%;
        text-align: center;
    }
    .clear{
        clear: both;
    }
</style>