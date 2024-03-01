<template>
	<view class="content">
		
	<view class="login-文字-area">
		<text class="login-文字">登录</text>
	</view>
	
	<view class="uni1">
		<view class="username-area">
			<text class="username">账号</text>
		</view>
		<view class="input-username-area">
			
			<input class="input-username" placeholder="请输入用户名" v-model="username"/>
			
		</view>
	</view>

		
	<view class="uni2">
		<view class="password-文字-area"><text class="password-文字">密码</text></view>
		<view class="input-password-area">
			<input class="input-password" placeholder="请输入密码" :password="showPassword" v-model="password"/>
			<text class="uni-icon" :class="[!showPassword ? 'uni-eye-active' : '']"
				@click="changePassword">&#xe568;</text>
		</view>
	</view>
				

	<view class="button-area">
		<button class="button" type='primary' @click="login">
			<view class="确认-文字">确认</view>
		</button>
	</view>
	
	<view class="进入方式-文字-area">
		<text class="进入方式-文字">其他进入方式</text>
	</view>
	
	<!-- <view class="图片1-area">
		<image class="图片1" src="../../static/wxx.png" mode="scaleToFill"></image>
	</view>
	<view class="图片2-area">
		<image class="图片2" src="../../static/qqq.png" mode="aspectFit"></image>
	</view>
	<view class="图片3-area">
		<image class="图片3" src="../../static/dyy.png" mode="aspectFit"></image>
	</view> -->
	
	<view class="点击注册-文字-area">
		<text class="点击注册-文字">没有账号？点击注册</text>
	</view>
	
	</view>
	
</template>

<script>
	export default {
		data() {
			return {
				username: '',
				password: '',
				form:{},
				showPassword: true
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
		 	},
			changePassword: function() {
			            this.showPassword = !this.showPassword;
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
		position: absolute;
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
	.uni1{
		/* Frame 9 */
		position: absolute;
		width: 325px;
		height: 74px;
		left: 22px;
		right: 28px;
		top: 138px;
		bottom: 600px;
		/* 自动布局 */
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: flex-start;
		padding: 0px;
		

	}
	.uni2{
		/* Frame 10 */
		position: absolute;
		width: 325px;
		height: 74px;
		left: 25px;
		right: 25px;
		top: 238px;
		bottom: 500px;
		/* 自动布局 */
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: flex-start;
		padding: 0px;
		

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
	.password-文字-area{
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
	.password-文字{
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
		border-radius: 6px;
		
		background: rgb(22, 33, 64);
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
		
		
		border-radius: 6px;
		background: rgb(95, 119, 245);
	}
	.button{
		
	}
	.确认-文字{
		
		/* Sign in */
		position: static;
		width: 41px;
		height: 32px;
		/* 自动布局 */
		display: flex;
		flex-direction: row;
		justify-content: center;
		align-items: center;
		padding: 0px 0px 0px 15px;
		
		
		/* Inside Auto Layout */
		flex: none;
		order: 0;
		flex-grow: 0;
		margin: 0px 10px;
		color: rgb(255, 255, 255);
		font-family: Poppins;
		font-size: 20px;
		font-weight: 600;
		line-height: 30px;
		letter-spacing: 0%;
		text-align: left;
	}
	
	.进入方式-文字-area{
		/* Access account */
		position: static;
		width: 96px;
		height: 24px;
		/* 自动布局 */
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 0px;
		
		
		/* Inside Auto Layout */
		flex: none;
		order: 0;
		flex-grow: 0;
		margin: 2px 0px;
	}
	.进入方式-文字{
		color: rgb(201, 201, 201);
		font-family: Poppins;
		font-size: 16px;
		font-weight: 400;
		line-height: 24px;
		letter-spacing: 0%;
		text-align: left;
	}
	.图片1-area{
		/* 1696428884254.png */
		position: absolute;
		width: 36px;
		height: 32px;
		left: 84px;
		right: 255px;
		top: 570px;
		bottom: 210px;
		border-radius: 15px;
		
		background: url();
	}
	.图片1{
		
	}
	.图片2-area{
		/* 1696429036445.png */
		position: absolute;
		width: 36px;
		height: 36px;
		left: 172px;
		right: 167px;
		top: 568px;
		bottom: 208px;
	}
	.图片2{
		border-radius: 24px;
		
		background: url();
	}
	.图片3-area{
		/* vector */
		position: absolute;
		width: 16.16px;
		height: 19.92px;
		left: 22.14%;
		right: 22.14%;
		top: 18.88%;
		bottom: 18.88%;
	}
	.图片3{
		background: rgb(255, 255, 255);
	}
	
	.进入方式-文字-area{
		/* Don’t have an account? Register */
		position: absolute;
		width: 108px;
		height: 18px;
		left: 133px;
		right: 134px;
		top: 736px;
		bottom: 58px;
	}
	.点击注册-文字{
		/* Don’t have an account? Register */
		position: absolute;
		width: 108px;
		height: 18px;
		left: 133px;
		right: 134px;
		top: 736px;
		bottom: 58px;
	}
	
</style>
