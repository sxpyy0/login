<template>
	<view class="content">
		<view class="register-文字-area">
			<text class="register-文字">注册</text>
		</view>
		<view class="phone-number-文字-area">
			<view class="phone-number-文字">请输入手机号</view>
		</view>
		<view class="input-phone-number-area">
			<uni-easyinput class="input-phone-number" v-model="form.phone_number"></uni-easyinput>
		</view>
		<view class="password-文字-area">
			<text class="password-文字">请输入密码</text>
		</view>
		<view class="input-password-area">
			<uni-easyinput class="input-password" type="password" v-model="form.password"></uni-easyinput>
		</view>
		<view class="confirm-password-文字-area">
			<text class="confirm-password-文字">请确认密码</text>
		</view>
		<view class="input-confirm-password-area">
			<uni-easyinput class="input-confirm-password" type="password" v-model="form.confirm_password"></uni-easyinput>
		</view>
		<view class="message-文字-area">
			<text class="message-文字">请输入短信验证码</text>
		</view>
		<view class="input-message-area">
			<uni-easyinput class="input-message" type="password" v-model="form.message"></uni-easyinput>
		</view>
		<view class="button-area">
			<button class="button" type='primary' @click="login">
				<view class="button-文字">注册</view>
			</button>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				form:{}
			}
		},
		methods: {
			login(){
				console.log(this.form)
			}
		}
	}
</script>

<style>
.content{
	/* Register */
	position: relative;
	width: 375px;
	height: 812px;
	background: rgb(7, 19, 51);
}
.register-文字-area{
	/* Register */
	position: absolute;
	width: 72px;
	height: 54px;
	left: 148px;
	right: 155px;
	top: 58px;
	bottom: 700px;
}
.register-文字{
	color: rgb(255, 255, 255);
	font-family: Poppins;
	font-size: 36px;
	font-weight: 600;
	line-height: 54px;
	letter-spacing: 0%;
	text-align: left;
}
.phone-number-文字-area{
	/* tele */
	position: static;
	width: 72px;
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
.phone-number-文字{
	color: rgb(201, 201, 201);
	font-family: Poppins;
	font-size: 12px;
	font-weight: 400;
	line-height: 18px;
	letter-spacing: 0%;
	text-align: left;
}
.input-phone-number-area{
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
.input-phone-number{
	border-radius: 6px;
	
	background: rgb(22, 33, 64);
}
.password-文字-area{
	/* Password */
	position: static;
	width: 60px;
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
.input-password{
	border-radius: 6px;
	
	background: rgb(22, 33, 64);
}
.confirm-password-文字-area{
	/* Password */
	position: static;
	width: 60px;
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
.confirm-password-文字{
	color: rgb(201, 201, 201);
	font-family: Poppins;
	font-size: 12px;
	font-weight: 400;
	line-height: 18px;
	letter-spacing: 0%;
	text-align: left;
}
.input-confirm-password-area{
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
.input-confirm-password{
	border-radius: 6px;
	
	background: rgb(22, 33, 64);
}
.message-文字-area{
	/* Password */
	position: static;
	width: 96px;
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
.message-文字{
	color: rgb(201, 201, 201);
	font-family: Poppins;
	font-size: 12px;
	font-weight: 400;
	line-height: 18px;
	letter-spacing: 0%;
	text-align: left;
}
.input-message-area{
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
.input-message{
	border-radius: 6px;
	
	background: rgb(22, 33, 64);
}
.button-area{
	/* Frame 8 */
	position: absolute;
	width: 325px;
	height: 56px;
	left: 25px;
	right: 25px;
	top: 568px;
	bottom: 188px;
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
	/* yes */
	position: static;
	
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
}
.button-文字{
	color: rgb(255, 255, 255);
	font-family: Poppins;
	font-size: 20px;
	font-weight: 600;
	line-height: 30px;
	letter-spacing: 0%;
	text-align: left;
}

</style>
