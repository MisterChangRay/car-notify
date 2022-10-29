<template>
	<view class="container">
		<uni-section title="联系人列表" type="line">
			<uni-list>
				<uni-list-item @click="callUser(item)" clickable v-for="(item, i ) in lists">
					<template v-slot:header>
						<view class="slot-box">
							<uni-icons type="phone" size="30"></uni-icons>
						</view>
					</template>
					<template v-slot:body>
						<text class="slot-box slot-text">点击拨号({{item}})</text>
					</template>
					<template v-slot:footer>
					</template>
				</uni-list-item>
				
			</uni-list>
		</uni-section>
	</view>
</template>

<script>
	export default {
		components: {},
		data() {
			return {
				lists:[]
			};
		},
		beforeMount() {
			var tels = this.GetQueryString("tel");
			this.lists = tels.split(",")
			console.log()
		},
		
		methods: {
			callUser(item) {
				console.log(item)
				uni.makePhoneCall({
					phoneNumber: item //仅为示例
				});
			},
			onClick(e) {
				console.log('执行click事件', e.data)
				uni.showToast({
					title: '点击反馈'
				});
			},
			GetQueryString (name) {
				var reg = new RegExp("(^|&)"+ name +"=([^&]*)(&|$)");
				var r = window.location.search.substr(1).match(reg);
				if(r!=null)return unescape(r[2]); return null;
			},
			switchChange(e) {
				uni.showToast({
					title: 'change:' + e.value,
					icon: 'none'
				});
			}
		}
	};
</script>

<style lang="scss">
	.slot-box {
		/* #ifndef APP-NVUE */
		display: flex;
		/* #endif */
		flex-direction: row;
		align-items: center;
	}

	.slot-image {
		/* #ifndef APP-NVUE */
		display: block;
		/* #endif */
		margin-right: 10px;
		width: 30px;
		height: 30px;
	}

	.slot-text {
		flex: 1;
		font-size: 14px;
		color: #4cd964;
		margin-right: 10px;
	}
</style>
