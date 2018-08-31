<template>
    <div class="topImgRoot">
        <img src="@/assets/tag1.jpg" class="mainImg">
        <div class="top">
            <div class="backContainer">
                <img src="@/assets/back.png" id="back" @click="toIndex">
            </div>
            <img src="@/assets/share.png" alt="" id="share">
        </div>
    </div>
</template>
<script>

    export default{
        data(){
            return {
                
            }
        },
        methods : {
            toIndex(){
                this.$router.push('/')
            }
        }
    }
</script>

<style>
.topImgRoot{

}
.topImgRoot .mainImg{
    width: 100%;
}
.topImgRoot .top{
    position: absolute;
    z-index: 10;
    top: 0;
    width: 100%;
    height: 25px;
    line-height: 25px;
}
.topImgRoot .backContainer{

}
.topImgRoot .backContainer img{
    height: 20px;
    position: relative;
    top: 10px;
    left: 10px;
}
.topImgRoot #share{
    float: right;
    position: relative;
    height: 20px;
    top: -15px;
    right: 10px;
}
</style>