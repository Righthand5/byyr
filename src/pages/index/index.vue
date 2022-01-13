<template>
	<view class="content">
		<image class="logo" src="/static/BYYR.png"></image>
    <input class="account" v-if="true" type="text" placeholder="请输入账号" />
    <input class="password" v-if="true" type="text" placeholder="请输入密码" />
    <view class="buttonwrapper">
      <button class="login button">登入</button>
      <button class="register button">注册</button>
    </view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style lang="scss" scoped>
	.content {
    height: 90vh;
		display: flex;
		flex-direction: column;
		align-items:center;
		justify-content:center;
	}

	.logo {
    width: 400rpx;
    height: 150rpx;
	}
	.account{
    width: 50vw;
    margin-top: 60rpx;
    box-shadow: 1px 1px 1px #888888;
  }
  .password{
    width: 50vw;
    margin-top: 30rpx;
    box-shadow: 1px 1px 1px #888888;
  }
  .buttonwrapper{
    display: flex;
    flex-direction: row;
    justify-content: center;
    justify-items: center;
    margin-top: 30rpx;
    .login{
      margin-right: 20rpx;
    }
  }
</style>
