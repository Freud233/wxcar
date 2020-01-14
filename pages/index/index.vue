<template>
	<view class="content">
		<view class="uni-padding-wrap">
			<view class="page-section swiper">
				<view class="page-section-spacing">
					<swiper class="swiper" :indicator-dots="indicatorDots" :autoplay="autoplay" :interval="interval" :duration="duration">
						<swiper-item>
							<view class="swiper-item uni-bg-red">
								<img src="http://pic1.win4000.com/wallpaper/5/582e95b20e3da.jpg" alt="">
							</view>
						</swiper-item>
						<swiper-item>
							<view class="swiper-item uni-bg-green">
								<img src="http://pic1.win4000.com/wallpaper/5/582e95b20e3da.jpg" alt="">
							</view>
						</swiper-item>
						<swiper-item>
							<view class="swiper-item uni-bg-blue">
								<img src="http://pic1.win4000.com/wallpaper/5/582e95b20e3da.jpg" alt="">
							</view>
						</swiper-item>
					</swiper>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				background: ['color1', 'color2', 'color3'],
				indicatorDots: true,
				autoplay: true,
				interval: 2000,
				duration: 500
			}
		},
		onLoad() {

		},
		methods: {
			changeIndicatorDots(e) {
				this.indicatorDots = !this.indicatorDots
			},
			changeAutoplay(e) {
				this.autoplay = !this.autoplay
			},
			intervalChange(e) {
				this.interval = e.target.value
			},
			durationChange(e) {
				this.duration = e.target.value
			}
		}
	}
</script>

<style lang="scss">
.swiper-item {
	img {
		width: 100%;
	}
}
</style>
