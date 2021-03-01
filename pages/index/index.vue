<template>
	<view>
		<swiper class="swiper" :indicator-dots='true' indicator-active-color="#000" autoplay='true' :interval="2000" >
			<swiper-item v-for="(item,index) of swiper" :key='index'>
				<image :src='item.url' ></image>
				<view>{{item.name}}</view>
			</swiper-item>
		</swiper>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				swiper:[
					{name:'A',url:'https://gimg2.baidu.com/image_search/src=http%3A%2F%2Fgss0.baidu.com%2F94o3dSag_xI4khGko9WTAnF6hhy%2Fzhidao%2Fpic%2Fitem%2F9825bc315c6034a85e771905c313495408237698.jpg&refer=http%3A%2F%2Fgss0.baidu.com&app=2002&size=f9999,10000&q=a80&n=0&g=0n&fmt=jpeg?sec=1617169846&t=fda5d557e265591bc5e0258fe1b07674'},
					{name:'B',url:'https://gimg2.baidu.com/image_search/src=http%3A%2F%2Fi-7.vcimg.com%2Ftrim%2F1dce9a40179f1949c08e5697e8041b7d130429%2Ftrim.jpg&refer=http%3A%2F%2Fi-7.vcimg.com&app=2002&size=f9999,10000&q=a80&n=0&g=0n&fmt=jpeg?sec=1617169887&t=3efaf824021e93816723db8de9e5e2d1'},
					{name:'C',url:'https://gimg2.baidu.com/image_search/src=http%3A%2F%2Fgss0.baidu.com%2F9vo3dSag_xI4khGko9WTAnF6hhy%2Fzhidao%2Fpic%2Fitem%2F9345d688d43f8794ed89fa93d21b0ef41bd53a1c.jpg&refer=http%3A%2F%2Fgss0.baidu.com&app=2002&size=f9999,10000&q=a80&n=0&g=0n&fmt=jpeg?sec=1617170449&t=b49c7bb9ccec57bf74b7bec44f8ba566'},
				]
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style lang='scss' scoped>
.swiper{
	height: 240px;
}
</style>
