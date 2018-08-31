<template>
    <div class="recommendPage">
        <div class="search">
            <img class="searchPng" src="@/assets/search.png">
            <span class="recommendSearch">X音乐</span>
            <span class="recommendSearch">X语言</span>
            <span class="recommendSearch">X美食</span>
            <img src="@/assets/saomiao.png" class="saomiao">
        </div>  
        <el-carousel height="185px">
            <el-carousel-item v-for="(item,ind) in tagList" :key="ind">
                <img :src="item.url" alt="" @click="toDetail">
            </el-carousel-item>
        </el-carousel>
    </div>
</template>
<script>
    export default{
        data(){
            return {
                tagList : [
                    {
                        url : require('@/assets/tag1.jpg')
                    },{
                        url : require('@/assets/tag2.jpg')
                    },{
                        url : require('@/assets/tag3.jpg')
                    },{
                        url : require('@/assets/tag4.jpg')
                    }
                ]
            }
        },
        methods : {
            toDetail(){
                this.$router.push('/detail')
            }
        }
    }
</script>
<style>
    .recommendPage .search{
        height: 25px;
        line-height: 25px;
        border: 1px #eaeaea solid;
        border-radius: 20px;
        text-align: center;
        background: #eaeaea;
    }
    .recommendPage img{
        width: 14px;
    }
    .recommendPage .searchPng{
        position: relative;
        top: 3px;
    }
    .recommendPage .recommendSearch{
        font-size: 10px;
        color: #8a8a8a;
        padding: 2px 8px;
    }
    .recommendPage .recommendSearch:nth-child(3){
        border-right: 1px solid #d4d4d4;
        border-left: 1px solid #d4d4d4;
    }
    .recommendPage .saomiao{
        float: right;
        position: relative;
        top: 6px;
        right: 15px;
    }
    .recommendPage .el-carousel{
        margin-top: 10px;
        border-radius: 5px;
    }
    .recommendPage .el-carousel__item{
        background: #99a9bf;
    } 
    .recommendPage .el-carousel__item img{
        width: 100%;
    }
</style>