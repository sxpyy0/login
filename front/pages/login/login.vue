<template>
	<view class="content">
		
	<view class="login-文字-area">
		<text class="login-文字">登录</text>
	</view>
	<view class="username-area">
		<text class="username">账号</text>
	</view>
	<view class="input-username-area">
		<uni-easyinput class="input-username" v-model="form.username" placeholder="请输入用户名"></uni-easyinput>
	</view>
	<view class="password-area">
		<text class="password">密码</text>
	</view>
	<view class="input-password-area">
		<uni-easyinput class="input-password" type="password" v-model="form.password" placeholder="请输入密码"></uni-easyinput>
	</view>
	<view class="button-area">
		<button class="button" type='primary' @click="login">确认</button>
	</view>
	
	</view>
	
</template>

<script>
	export default {
		data() {
			return {
				// username: '',
				// password: '',
				form:{}
			}
		},
		methods: {
			login(){
				console.log(this.form)
				// const baseUrl="htts://localhost:9090"
				// uni.request({
				// 	url:,
				// 	method:"POST",
				// 	data:this.form,
				// 	success: (res) => {
				// 		const data=res.data
				// 		if(data.code!=='200'){
				// 			uni.showToast({
				// 				icon:"none",
				// 				title:data.msg
				// 			})
				// 		} else{
				// 			uni.navigateTo({
				// 				url:'/pages/index/index'
				// 			})
				// 			uni.showToast({
				// 				title:'登录成功'
				// 			})
				// 			//存储用户数据到storage
				// 			uni.setStorageSync('user',data.data)
				// 		}
				// 	}
				// })
		 	}
		 }
	}
</script>

<style>
	.content{
		/* Login */
		position: relative;
		width: 375px;
		height: 812px;
		background: rgb(7, 19, 51);
	}
	.login-文字-area{
		/* Login */
		position: relative;
		width: 72px;
		height: 54px;
		left: 148px;
		right: 155px;
		top: 58px;
		bottom: 700px;
	}
	.login-文字{
		color: rgb(255, 255, 255);
		font-family: Poppins;
		font-size: 36px;
		font-weight: 600;
		line-height: 54px;
		letter-spacing: 0%;
		text-align: left;
	}
	.username-area{
		/* Email */
		position: static;
		width: 24px;
		height: 18px;
		/* 自动布局 */
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: flex-start;
		padding: 0px;
		
		
		/* Inside Auto Layout */
		flex: none;
		order: 0;
		flex-grow: 0;
		margin: 11px 0px;
	}
	.username{
		color: rgb(201, 201, 201);
		font-family: Poppins;
		font-size: 12px;
		font-weight: 400;
		line-height: 18px;
		letter-spacing: 0%;
		text-align: left;
	}
	.password-area{
		/* Password */
		position: static;
		width: 24px;
		height: 18px;
		/* 自动布局 */
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: flex-start;
		padding: 0px;
		
		
		/* Inside Auto Layout */
		flex: none;
		order: 0;
		flex-grow: 0;
		margin: 11px 0px;
	}
	.password{
		color: rgb(201, 201, 201);
		font-family: Poppins;
		font-size: 12px;
		font-weight: 400;
		line-height: 18px;
		letter-spacing: 0%;
		text-align: left;
	}
	.input-username-area{
		/* Frame 8 */
		position: static;
		width: 325px;
		height: 45px;
		/* 自动布局 */
		display: flex;
		flex-direction: row;
		justify-content: flex-start;
		align-items: center;
		padding: 0px 0px 0px 15px;
		
		
		/* Inside Auto Layout */
		flex: none;
		order: 1;
		flex-grow: 0;
		margin: 11px 0px;
		
		border-radius: 6px;
		
		background: rgb(22, 33, 64);
	}
	
	.input-password-area{
		/* Frame 8 */
		position: static;
		width: 325px;
		height: 45px;
		/* 自动布局 */
		display: flex;
		flex-direction: row;
		justify-content: flex-start;
		align-items: center;
		padding: 0px 0px 0px 15px;
		
		
		/* Inside Auto Layout */
		flex: none;
		order: 1;
		flex-grow: 0;
		margin: 11px 0px;
	}
	
	
	.button-area{
		/* Frame 8 */
		position: absolute;
		width: 325px;
		height: 56px;
		left: 22px;
		right: 28px;
		top: 350px;
		bottom: 406px;
		/* 自动布局 */
		display: flex;
		flex-direction: row;
		justify-content: center;
		align-items: center;
		padding: 0px 0px 0px 15px;
	}
	.button{
		border-radius: 6px;
		background: rgb(95, 119, 245);
	}
</style>
