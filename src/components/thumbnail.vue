<template>
    <div class="thumbnailRoot">
        <div class="thumbanil"  v-for="(data,ind) in listData" :key="ind">
            <div class="thumbanilImg">
                <img :src="data.imgUrl" alt="">
            </div>
            <div class="title">{{data.title}}</div>
        </div>
    </div>
    
</template>
<script>
    export default{
        // props : ['listData'],
        data(){
            return {
                listData : [
                    {
                        imgUrl : require('../assets/xMen.jpg'),
                        title : 'xMen : 在路上的音乐故事'
                    },{
                        imgUrl : require('../assets/xWomen.jpg'),
                        title : 'xWomen : 在他乡'
                    },{
                        imgUrl : require('@/assets/guodegang.jpg'),
                        title : '今天模仿郭德纲'
                    },{
                        imgUrl : require('@/assets/thum2.jpg'),
                        title : '总有这样的歌只想一个人听'
                    },{
                        imgUrl : require('@/assets/thum3.jpg'),
                        title : '一段话 一首歌'
                    },{
                        imgUrl : require('@/assets/thum4.jpg'),
                        title : '深夜小茶馆'
                    }
                ]
            }
        }
    }
</script>
<style>
    .thumbnailRoot{
        margin-top: 20px;
    }
    .thumbnailRoot .thumbanil{
        width: 45%;
        display: inline-block;
        padding: 0 2%;
    }
    .thumbnailRoot .thumbanil .thumbanilImg{
        height: 155px;
        border-radius: 8px;
    }
    .thumbnailRoot .thumbanil .thumbanilImg img{
        width: 100%;
        height: 150px;
    }
    .thumbnailRoot .thumbanil .title{
        overflow: hidden;
        text-overflow:ellipsis;
        white-space: nowrap;
        margin-top: 5px;
        font-size: 12px;
        color: #444;
    }
</style>