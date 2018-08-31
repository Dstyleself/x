<template>
    <div class="root">
        <top-tag></top-tag>
		<recommend-page class=""></recommend-page>
        <thum-bnail></thum-bnail>
    </div>
</template>
<script>

    import topTag from '@/components/topTag'
    import recommendPage from '@/components/recommendPage'
    import thumBnail from '@/components/thumbnail'
    export default {
        components : {
            topTag,
            recommendPage,
            thumBnail
        }
    }
</script>
<style>
.root{
    padding: 0 8px;
}
</style>