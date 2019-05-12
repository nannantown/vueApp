
<template>
	<view>
		<text class="text-color-primary">{{message}}</text>
		<button :title="btnMessage" :on-press="handleClick" />
		<text>{{clickCount}}</text>
	</view>
</template>

<script>
	export default {
		data (){
			return {
				message: 'Welcome to my application',
				btnMessage: 'Click Me',
				clickCount: 0
			}
		},
		methods: {
			handleClick () {
				this.clickCount ++
			}
		}
	}
</script>

<style>

.text-color-primary {
  color: blue;
}
</style>