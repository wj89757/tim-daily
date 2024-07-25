<template>
	<view>
		<uni-section title="" padding>
			<uni-grid :column="2" :highlight="true" @change="change" showBorder="false" borderColor="#fff">
				<uni-grid-item v-for="(item, index) in 32" :index="index" :key="index">
					<view class="grid-item-box" style="background-color: #fff">
						<image style="width: 100%; height: 100%;" mode="aspectFill"
							src="https://danqing.163.com/backend-outer/vlp/dqy_1721644227.503648ComfyUI_temp_zapmk_00001_.png?Signature=dyPOy4CNb1E6Ut%2FuGyLQm7boy7I%3D&Expires=2037004227&AWSAccessKeyId=J0QA8PBPBX2SKQYYDY8X">
						</image>
						<text class="text">很好的好的好的回电话</text>
					</view>
				</uni-grid-item>
			</uni-grid>
		</uni-section>
	</view>
</template>

<script>
	export default {
		data() {
			return {

			}
		},
		methods: {

		}
	}
</script>

<style>
	.grid-item-box {
		flex: 1;
		// position: relative;
		/* #ifndef APP-NVUE */
		display: flex;
		/* #endif */
		flex-direction: column;
		align-items: left;
		justify-content: center;
		overflow: hidden;
		margin: 10px;
		box-shadow: 0px 10px 15px -3px rgba(0,0,0,0.1),0px 10px 15px -3px rgba(0,0,0,0.1);
	}

	.text {
		white-space: nowrap;
		overflow: hidden;
		text-overflow: ellipsis;
		padding-left: 3%;
	}

	/* #ifdef H5 */
	@media screen and (min-width: 768px) and (max-width: 1425px) {
		.swiper {
			height: 630px;
		}
	}

	@media screen and (min-width: 1425px) {
		.swiper {
			height: 830px;
		}
	}

	/* #endif */
</style>