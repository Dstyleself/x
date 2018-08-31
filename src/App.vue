<template>
	<div id="app">	
		 <transition enter-active-class="bounceInLeft animated">
            <router-view class="routerview"></router-view>
          </transition>
		<!-- <router-view/> -->
	</div>
</template>

<script>

export default {
    name: 'App',
	components : {
		
	}
}
</script>

<style>
</style>
