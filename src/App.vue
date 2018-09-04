<template>
	<div id="app">	
		<transition enter-active-class="bounceInLeft animated">
            <router-view class="routerview"></router-view>
        </transition>
		<bottom-tag></bottom-tag>
		<!-- <router-view/> -->
	</div>
</template>

<script>
import bottomTag from '@/components/bottom'
export default {
    name: 'App',
	components : {
		bottomTag
	}
}
</script>

<style>
</style>
