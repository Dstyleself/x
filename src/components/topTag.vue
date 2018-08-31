<template>
    <div class="topTag">
        <ul>
            <li v-for="(item,ind) in tagList" :to="item.tagPath" :key="ind">{{item.tagName}}</li>
        </ul>
    </div>
</template>
<script>
export default{
    data(){
        return {
            tagList : [
                {
                    tagName : '推荐',
                    tagPath : '/recommendPage'
                },{
                    tagName : '本地电台',
                    tagPath : '/locationRadio'
                },{
                    tagName : 'x音乐',
                    tagPath : '/music'
                },{
                    tagName : 'x美食',
                    tagPath : '/cate'
                },{
                    tagName : 'x语言',
                    tagPath : '/language'
                },{
                    tagName : 'x游戏',
                    tagPath : '/game'
                }
            ]
        }
    }
}
</script>
<style>
.topTag{
    height: 50px;
    line-height: 50px;
}
.topTag ul{
    padding-left: 0px;
}
.topTag ul li{
    float: left;
    list-style-type: none;
    padding: 0 13px;
    /* line-height: 50px; */
    font-size: 14px;
    color: #444;
    cursor: pointer;
}
</style>