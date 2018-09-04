<template>
    <div class="playerRoot">
        <img src="@/assets/stop.png" class="stopImg" alt="">
        <span class="progressBar"></span>
        <span class="time">1:22:49</span>
    </div>
</template>
<script>

    export default{

    }
</script>

<style>
    .playerRoot .stopImg{
        margin-left: 10px;
        width: 25px;
        position: relative;
        top: 7px;
    }
    .playerRoot .progressBar{
        display: inline-block;
        width: 75%;
        border: 1px #fff solid;
        position: relative;
        top: -3px;
        left: 8px;
    }
    .playerRoot .time{
        margin-left: 10px;
        color: #fff;
        font-size: 12px;
    }
</style>